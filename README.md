# Li-Pro.Net static artifacts for Sphinx documents

This repository contains static artifacts shared with multiple Sphinx
document projects.

## Checkout repository

Since the project utilizes the reuse of other Git repositories through
Git submodules, one must also pay attention to these when cloning. Using
different Git versions results in different calls to do this.

With **version 2.13 of Git and later**, `--recurse-submodules` can be used
instead of `--recursive`:

```sh
git clone --recurse-submodules git@github.com:lipro/lpn-sphinx_static.git
cd core
```

With **version 1.6.5 of Git up until version 2.12**, you can use:

```sh
git clone --recursive git@github.com:lipro/lpn-sphinx_static.git
cd core
```

For already cloned repos, or older Git versions, use:

```sh
git clone git@github.com:lipro/lpn-sphinx_static.git
cd core
git submodule update --init --recursive
```

## Setup build environment

Only needed at once when you start.

### Linux

Install arbitrary tools first:

```sh
sudo apt install \
         woff2 \
         eot-utils \
         fontconfig \
         fontforge-nox \
```

### MacOS and Windows

*not supported*
