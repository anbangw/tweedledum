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

### Other Stuffs

[Original README](./README1.md)