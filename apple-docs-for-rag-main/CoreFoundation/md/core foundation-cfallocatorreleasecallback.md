

- Core Foundation
-  CFAllocatorReleaseCallBack 

Type Alias

# CFAllocatorReleaseCallBack

A prototype for a function callback that releases the given data.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFAllocatorReleaseCallBack = (UnsafeRawPointer?) -> Void
```

## Parameters 

`info`  

The data to be released.

## Discussion

A prototype for a function callback that releases the data pointed to by the `info` field. In implementing this function, release (or free) the data you have defined for the allocator context.

## See Also

### Callbacks

typealias CFAllocatorAllocateCallBack

A prototype for a function callback that allocates memory of a requested size.

typealias CFAllocatorCopyDescriptionCallBack

A prototype for a function callback that provides a description of the specified data.

typealias CFAllocatorDeallocateCallBack

A prototype for a function callback that deallocates a block of memory.

typealias CFAllocatorPreferredSizeCallBack

A prototype for a function callback that gives the size of memory likely to be allocated, given a certain request.

typealias CFAllocatorReallocateCallBack

A prototype for a function callback that reallocates memory of a requested size for an existing block of memory.

typealias CFAllocatorRetainCallBack

A prototype for a function callback that retains the given data.

