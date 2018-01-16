# OpenEmbedded/Yocto layer with compiler ports

This layer aims at porting some old compilers to newer Yocto releases.

## Why?

Because sometimes an old compiler is required, but you still want to use more updated recipes and OE system
than the ones shipped with the release which supports your compiler.

## Compilers tested

Unless otherwise specified, tests involve building a fully functional image using Poky as a reference distribution.

| Compiler 	| Rocko |
| --- 		| :---:	|
| GCC 4.9 	| V 	|

## Dependencies

This layer depends on:
URI: git://git.openembedded.org/openembedded-core
branch: rocko

# Contributing

Please submit issues and pull requests via GitHub.
