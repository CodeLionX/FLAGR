# (Py)FLAGR

* Fuse, Learn, AGgregate, Rerank



The fusion of multiple ranked lists of elements into a single aggregate list is a well-studied research field with numerous applications in Bioinformatics, recommendation systems, collaborative filtering, election systems and metasearch engines.

FLAGR is a high performance, modular, open source C++ library for rank aggregation problems. It implements baseline and recent state-of-the-art aggregation algorithms that accept ranked preference lists and generate a single consensus list of elements. A portion of these methods apply exploratory analysis techniques and belong to the broad family of unsupervised learning techniques.

PyFLAGR is a Python library built on top of FLAGR library core. It can be easily installed with pip (see below) and used in standard Python programs and Jupyter notebooks. Representative code examples can be found on [this notebook](https://github.com/lakritidis/FLAGR/blob/main/README.ipynb).

The current FLAGR version is 1.0.8.

Both libraries are licensed under the Apache License, version 2.

The library is fully documented at [https://flagr.site/](https://flagr.site/)


## Compiling from Sources

FLAGR can be easily compiled from its C++ sources by using the provided build scripts. The scripts require a working GCC compiler to be installed into the machine that performs the compilation.

There are two build scripts, one for Linux and one for Windows. Specifically:

* In Linux: type `make` in the terminal to build the binaries from the C++ sources. The FLAGR executable file is automatically created into the `bin/Release/` directory of the package. In addition, a shared `.so` library will be created into `bin/Release/` and `pyflagr/pyflagr/`.
* In Windows: type `makefile.bat` in Windows CLI or Windows Powershell. The batch file will build the binaries from the C++ sources and generate `FLAGR.exe` into the `bin/Release/` directory. Moreover, a Dynamic Link `.dll` Library will be created  into `bin/Release/` and `pyflagr/pyflagr/`.



## Installing PyFLAGR

PyFLAGR can be installed directly by using `pip`:

`pip install pyflagr`

Alternatively, PyFLAGR can be installed from the sources by navigating to the directory where `setup.py` resides:

`pip install .`

