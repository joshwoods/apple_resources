

- Core Foundation
-  CFAllocatorContext 

Structure

# CFAllocatorContext

A structure that defines the context or operating environment for an allocator (CFAllocator) object. Every Core Foundation allocator object must have a context defined for it.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CFAllocatorContext
```

## Overview

See the Memory Management Programming Guide for Core Foundation topic for information on creating a custom CFAllocator object and, as part of that procedure, the steps for creating a properly initialized `CFAllocatorContext` structure.

## Topics

### Initializers

init()

init(version: CFIndex, info: UnsafeMutableRawPointer!, retain: CFAllocatorRetainCallBack!, release: CFAllocatorReleaseCallBack!, copyDescription: CFAllocatorCopyDescriptionCallBack!, allocate: CFAllocatorAllocateCallBack!, reallocate: CFAllocatorReallocateCallBack!, deallocate: CFAllocatorDeallocateCallBack!, preferredSize: CFAllocatorPreferredSizeCallBack!)

### Instance Properties

var allocate: CFAllocatorAllocateCallBack!

A prototype for a function callback that allocates memory of a requested size. In implementing this function, allocate a block of memory of at least `size` bytes and return a pointer to the start of the block. The `hint` argument is a bitfield that you should currently not use (that is, assign 0). The `size` parameter should always be greater than 0. If it is not, or if problems in allocation occur, return `NULL`. This function pointer may not be assigned `NULL`.

var copyDescription: CFAllocatorCopyDescriptionCallBack!

A prototype for a function callback that provides a description of the data pointed to by the `info` field. In implementing this function, return a reference to a CFString object that describes your allocator, particularly some characteristics of your program-defined data. You may set this function pointer to `NULL`, in which case Core Foundation will provide a rudimentary description.

var deallocate: CFAllocatorDeallocateCallBack!

A prototype for a function callback that deallocates a given block of memory. In implementing this function, make the block of memory pointed to by `ptr` available for subsequent reuse by the allocator but unavailable for continued use by the program. The `ptr` parameter cannot be `NULL` and if the `ptr` parameter is not a block of memory that has been previously allocated by the allocator, the results are undefined; abnormal program termination can occur. You can set this callback to `NULL`, in which case the CFAllocatorDeallocate(_:_:) function has no effect.

var info: UnsafeMutableRawPointer!

An untyped pointer to program-defined data. Allocate memory for this data and assign a pointer to it. This data is often control information for the allocator. You may assign `NULL`.

var preferredSize: CFAllocatorPreferredSizeCallBack!

A prototype for a function callback that determines whether there is enough free memory to satisfy a request. In implementing this function, return the actual size the allocator is likely to allocate given a request for a block of memory of size `size`. The `hint` argument is a bitfield that you should currently not use.

var reallocate: CFAllocatorReallocateCallBack!

A prototype for a function callback that reallocates memory of a requested size for an existing block of memory.

var release: CFAllocatorReleaseCallBack!

A prototype for a function callback that releases the data pointed to by the `info` field. In implementing this function, release (or free) the data you have defined for the allocator context. You may set this function pointer to `NULL`, but doing so might result in memory leaks.

var retain: CFAllocatorRetainCallBack!

A prototype for a function callback that retains the data pointed to by the `info` field. In implementing this function, retain the data you have defined for the allocator context in this field. (This might make sense only if the data is a Core Foundation object.) You may set this function pointer to `NULL`.

var version: CFIndex

An integer of type `CFIndex`. Assign the version number of the allocator. Currently the only valid value is 0.

## Relationships

### Conforms To

- BitwiseCopyable

