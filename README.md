About
=========

A modified unsquashfs utility that attempts to support as many hacked-up vendor-specific SquashFS implementations as possible.

If the vendor has done something simple like just muck a bit with the header fields, this tool should sort it out.

If the vendor has made changes to the underlying LZMA compression options, or how these options are stored in the compressed data blocks, this tool will attempt to resolve such customizations via a brute-force method.

Very beta.

Prerequisites
=============

You need a C/C++ compiler, plus the liblzma and zlib development libraries.

Modified Files
==============

The following files have been modified from their original version. They have been formatted to fit your screen:

 * compressor.c
 * compressor.h
 * error.h
 * lzma_wrapper.c
 * Makefile
 * process_fragments.c
 * read_fs.c
 * squashfs_fs.h
 * unsquashfs.c
 * LZMA/lzmalt/LZMADecoder.c
 * LZMA/lzmadaptive/C/7zip/Compress/LZMA_Lib/ZLib.cpp
 * LZMA/lzmadaptive/C/7zip/Compress/LZMA_Lib/lzmadaptive.h

