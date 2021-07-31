# LabGraph

LabGraph is a streaming framework built by the Facebook Reality Labs Research team at Facebook. More information can be found [here](docs/index.md).

## Quick Start

### Method 1 - using PyPI (Recommended)

**Prerequisites**:
- [Python 3.6](https://www.python.org/downloads/release/python-368/)
- Windows and Linux (CentOS 7, CentOS 8, Ubuntu 20.04)
- Based on [PyPa](https://github.com/pypa/manylinux), the following Linux system is also supported: Fedora 32+, Mageia 8+, openSUSE 15.3+, Photon OS 4.0+ (3.0+ with updates), Ubuntu 20.04+

```
pip install labgraph
```

### Method 2 - building from source code

**Prerequisites**:

- [Buck](https://buck.build/setup/getting_started.html) ([Watchman](https://facebook.github.io/watchman/docs/install) also recommended)
- [Python 3.6](https://www.python.org/downloads/release/python-368/) (note: currently incompatible with Anaconda)
- **Windows only:** [Build Tools for Visual Studio 2019](https://visualstudio.microsoft.com/downloads/#build-tools-for-visual-studio-2019)

**Setup**:

*On Windows, this setup step must be run in "x64 Native Tools Command Prompt for VS 2019" so that we can access the Visual Studio compiler toolchain.*

```
cd labgraph
python setup.py install
```

### Testing:

To make sure things are working you can run the example:

```
python -m labgraph.examples.simple_viz
```

You can also run the test suite as follows:

```
python -m pytest --pyargs labgraph
```
or (for some Linux users)

```
RUN export LC_ALL=C.UTF-8
RUN export LANG=en_US.utf-8
. test_script.sh
```

Now go to the [index](docs/index.md) and [documentation](docs/) to learn more!


**License**:
LabGraph is MIT licensed, as found in the LICENSE file.
