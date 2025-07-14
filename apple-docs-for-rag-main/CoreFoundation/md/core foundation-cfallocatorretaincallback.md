

- Core Foundation
-  CFAllocatorRetainCallBack 

Type Alias

# CFAllocatorRetainCallBack

A prototype for a function callback that retains the given data.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFAllocatorRetainCallBack = (UnsafeRawPointer?) -> UnsafeRawPointer?
```

## Parameters 

`info`  

The data to be retained.

## Discussion

A prototype for a function callback that retains the data pointed to by the `info` field. In implementing this function, retain the data you have defined for the allocator context in this field. (This might make sense only if the data is a Core Foundation object.)

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

typealias CFAllocatorReleaseCallBack

A prototype for a function callback that releases the given data.

