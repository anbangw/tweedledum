## Tweedledum

This fork fixes the compilation of tweedledum on Linux x64 and aarch64 platform. 

### Tested Platform

Ubuntu aarch64 24.04. Miniconda Python 3.12.2.
If reporting errors like `libstdc++.so.6: version GLIBCXX_3.4.20 not found`, run the following command: 
```bash
conda install -c conda-forge libstdcxx-ng
```


Ubuntu x64 24.04

[Original README](./README1.md)