

- Kernel
-  libkern 

API Collection

# libkern

Access the runtime support and base classes of the kernel library.

## Topics

### Fundamentals

Data Types

Create strings, numbers, collections, data objects, and the other standard types employed by drivers and kernel extensions.

Atomic Operations

Increment and decrement numbers, perform compare-and-swap operations, and manipulate other data atomically.

Byte Order Utilities

Convert values between big-endian and little-endian formats.

### Memory

OSMalloc

Allocates a block of memory associated with a given OSMallocTag.

OSMalloc_Tagalloc

Creates a tag for use with OSMalloc functions.

OSMalloc_Tagfree

Frees a tag used with OSMalloc functions.

OSMalloc_noblock

Allocates a block of memory associated with a given OSMallocTag, returning `NULL` if it would block.

OSMalloc_nowait

Equivalent to OSMalloc_noblock.

OSFree

Frees a block of memory allocated by OSMalloc.

bzero

bzero_phys

### Compression

deflate

deflateBound

deflateCopy

deflateEnd

deflateInit2_

deflateInit_

deflateParams

deflatePrime

deflateReset

deflateSetDictionary

deflateSetHeader

deflateTune

inflate

inflateBack

inflateBackEnd

inflateBackInit_

inflateCopy

inflateEnd

inflateGetHeader

inflateInit2_

inflateInit_

inflatePrime

inflateReset

inflateSetDictionary

inflateSync

inflateSyncPoint

compress

compress2

compressBound

adler32

adler32_combine

### Cryptography

MD5_CTX

MD5Final

MD5Init

MD5Update

### Non Quad Routines

fls

flsll

ffs

ffsll

### copyio

copyin

copyinstr

copyout

copyoutstr

copystr

## See Also

### IOKit Drivers

IOKit Fundamentals

Implement a driver for your custom hardware using a third-party kernel extension.

Hardware Families

Add support for specific hardware protocols such as USB, and for standard network, serial, audio, and graphics interfaces.

Driver Support

Explore the device registry and access power-management utilities and other shared driver features.

