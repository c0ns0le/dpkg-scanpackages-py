# dpkg-scanpackages.py

A Python implementation of Debian's `dpkg-scanpackages`.

## Requirements

This script requires [python-dpkg](https://github.com/TheClimateCorporation/python-dpkg). Install from [PyPi](https://pypi.python.org/) using the [pip](https://packaging.python.org/installing/) tool:

```
pip install pydpkg
```

## Usage

```
Usage: python dpkg-scanpackages.py <binary-path> > Packages

Options:
  -?, --help               show this help message. 
      --version            show the version.
```

## Caveats

* On Windows™, piping the output to a file results into a file with CRLF endings. File must me converted to unix-style (LF) line endings before using in an apt repo. 

## Changelog

* v0.1.1
    + variable name correction 
* v0.1.0
    + Base functionality. No switches available besides `--help` and `--version`