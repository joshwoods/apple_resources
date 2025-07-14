

- Core Foundation
-  CFAllocatorAllocateCallBack 

Type Alias

# CFAllocatorAllocateCallBack

A prototype for a function callback that allocates memory of a requested size.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFAllocatorAllocateCallBack = (CFIndex, CFOptionFlags, UnsafeMutableRawPointer?) -> UnsafeMutableRawPointer?
```

## Parameters 

`allocSize`  

This function allocates a block of memory of at least `allocSize` bytes (always greater than 0).

`hint`  

A bitfield that is currently not used (always set to 0).

`info`  

An untyped pointer to program-defined data. Allocate memory for the data and assign a pointer to it. This data is often control information for the allocator. It may be `NULL`.

## Return Value

A pointer to the start of the block.

## See Also

### Callbacks

typealias CFAllocatorCopyDescriptionCallBack

A prototype for a function callback that provides a description of the specified data.

typealias CFAllocatorDeallocateCallBack

A prototype for a function callback that deallocates a block of memory.

typealias CFAllocatorPreferredSizeCallBack

A prototype for a function callback that gives the size of memory likely to be allocated, given a certain request.

typealias CFAllocatorReallocateCallBack

A prototype for a function callback that reallocates memory of a requested size for an existing block of memory.

typealias CFAllocatorReleaseCallBack

A prototype for a function callback that releases the given data.

typealias CFAllocatorRetainCallBack

A prototype for a function callback that retains the given data.

