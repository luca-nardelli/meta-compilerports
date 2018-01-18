# OpenEmbedded/Yocto layer with compiler ports

This layer aims at porting some old compilers to newer Yocto releases.

## Why?

Because sometimes an old compiler is required, but you still want to use more updated recipes and OE system
than the ones shipped with the release which supports your compiler.

After a long time working on the Jethro release on a CUDA 6.5 platform (Jetson TK1) which requires GCC 4.X I wanted to upgrade to a newer Yocto release, and this asked for a porting of the compiler recipes. 

## Structure

This layer is composed of some sub-layers:
* meta-compilers holds the actual GCC recipes
* meta-`compilername` holds some bbappends for recipes that failed building when using `compilername`. Note that this list is not inclusive of all packages, it gets updated whenever a new incompatible package is found.

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
