## Tweedledum

This fork fixes the compilation of tweedledum on Linux x64 and aarch64 platform. 

### INSTALL

Download the repo, then

```bash
cd tweedledum
pip install .
```

### Tested Platform

Ubuntu aarch64 24.04. Miniconda Python 3.12.2.
If reporting errors like `libstdc++.so.6: version GLIBCXX_3.4.20 not found`, run the following command: 
```bash
conda install -c conda-forge libstdcxx-ng
```


Ubuntu x64 24.04.

### Modification

1. This fork deletes the `[project]` section in the pyproject.toml file for newer setuptools
2. This fork adds a line `#include <cstdint>` to the `include/tweedledum/IR/Cbit.h` to resolve errors like `uint32_t does not name a type` on the aarch64 platform.
3. This fork updates pybind11 to the version 2.13.6. Python 3.12 removes PyFrameObject, so needing a newer version of pybind11 to avoid compilation problems.

### Other Stuffs

[Original README](./README1.md)