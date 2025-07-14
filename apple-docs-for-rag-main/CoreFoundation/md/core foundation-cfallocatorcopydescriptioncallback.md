

- Core Foundation
-  CFAllocatorCopyDescriptionCallBack 

Type Alias

# CFAllocatorCopyDescriptionCallBack

A prototype for a function callback that provides a description of the specified data.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFAllocatorCopyDescriptionCallBack = (UnsafeRawPointer?) -> Unmanaged?
```

## Parameters 

`info`  

An untyped pointer to program-defined data.

## Return Value

A CFString object that describes the allocator. The caller is responsible for releasing this object.

## Discussion

A prototype for a function callback that provides a description of the data pointed to by the `info` field. In implementing this function, return a reference to a CFString object that describes your allocator, particularly some characteristics of your program-defined data.

## See Also

### Callbacks

typealias CFAllocatorAllocateCallBack

A prototype for a function callback that allocates memory of a requested size.

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

