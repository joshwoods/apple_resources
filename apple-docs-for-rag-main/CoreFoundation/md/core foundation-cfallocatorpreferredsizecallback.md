

- Core Foundation
-  CFAllocatorPreferredSizeCallBack 

Type Alias

# CFAllocatorPreferredSizeCallBack

A prototype for a function callback that gives the size of memory likely to be allocated, given a certain request.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFAllocatorPreferredSizeCallBack = (CFIndex, CFOptionFlags, UnsafeMutableRawPointer?) -> CFIndex
```

## Parameters 

`size`  

The amount of memory requested.

`hint`  

A bitfield that is currently not used (always set to 0).

`info`  

An untyped pointer to program-defined data.

## Return Value

The actual size the allocator is likely to allocate given this request.

## Discussion

A prototype for a function callback that determines whether there is enough free memory to satisfy a request. In implementing this function, return the actual size the allocator is likely to allocate given a request for a block of memory of size `size`. The `hint` argument is a bitfield that you should currently not use.

## See Also

### Callbacks

typealias CFAllocatorAllocateCallBack

A prototype for a function callback that allocates memory of a requested size.

typealias CFAllocatorCopyDescriptionCallBack

A prototype for a function callback that provides a description of the specified data.

typealias CFAllocatorDeallocateCallBack

A prototype for a function callback that deallocates a block of memory.

typealias CFAllocatorReallocateCallBack

A prototype for a function callback that reallocates memory of a requested size for an existing block of memory.

typealias CFAllocatorReleaseCallBack

A prototype for a function callback that releases the given data.

typealias CFAllocatorRetainCallBack

A prototype for a function callback that retains the given data.

