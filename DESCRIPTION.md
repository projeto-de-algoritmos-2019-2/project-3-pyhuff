# PyHuff 
[![PyPI](https://img.shields.io/pypi/v/pyhuff)](https://pypi.org/project/pyhuff/) [![format](https://img.shields.io/pypi/format/pyhuff)](https://pypi.org/project/pyhuff/)

## Description
This package allows its users to shrink any ASCII based file using Huffman Code algorithm.

---

## Installing
PyHuff is available in [PyPi](https://pypi.org/project/pyhuff/):
```sh
$ pip install pyhuff
```

---

## Usage
To shrink a file named `example.txt`:
```sh
$ pyhuff example.txt
```

Two files will be created:
- **example.huff**: the encoded file
- **example.tree.huff**: the huffman tree used to encode the file

To restore the original file:
```sh
$ pyhuff example.huff example.tree.huff decoded_example.txt
```
In the example above, the decoded file will be created as `decoded_example.txt`. You can pass any filename as argument. Notice that, if the given file already exists, it will be overwritten.

To get help, simply call:
```sh
$ pyhuff
```
---

created by [Durval Carvalho](https://github.com/durvalcarvalho) and [Victor Moura](https://github.com/victorcmoura)
