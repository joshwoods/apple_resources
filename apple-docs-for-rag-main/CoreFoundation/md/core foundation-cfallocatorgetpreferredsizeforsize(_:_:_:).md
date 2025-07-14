

- Core Foundation
-  CFAllocatorGetPreferredSizeForSize(\_:\_:\_:) 

Function

# CFAllocatorGetPreferredSizeForSize(\_:\_:\_:)

Obtains the number of bytes likely to be allocated upon a specific request.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFAllocatorGetPreferredSizeForSize(
    _ allocator: CFAllocator!,
    _ size: CFIndex,
    _ hint: CFOptionFlags
) -> CFIndex
```

## Parameters 

`allocator`  

The allocator to use, or `NULL` for the default allocator.

`size`  

The number of bytes to allocate. If the value is `0` or less, the result is the same value.

`hint`  

A bitfield of type `CFOptionsFlags`. Pass flags to the allocator that suggest how memory is to be allocated. `0` indicates no hints. No hints are currently defined, only `0` should be passed for this argument.

## Return Value

The number of bytes likely to be allocated upon a specific request.

## Discussion

The return value depends on the allocator’s internal allocation strategy, and will be equal to or larger than `size`. Calling this function may help you better match your memory allocation or reallocation strategy to that of the allocator.

Note that the return value depends on the internal implementation of the allocator and the results may change from release to release or from platform to platform.

If no function callback is assigned to the `preferredSize` field of the allocator’s context (see the `CFAllocatorContext` structure), then the value of `size` is returned.

## See Also

### Managing Memory with an Allocator

func CFAllocatorAllocate(CFAllocator!, CFIndex, CFOptionFlags) -> UnsafeMutableRawPointer!

Allocates memory using the specified allocator.

func CFAllocatorDeallocate(CFAllocator!, UnsafeMutableRawPointer!)

Deallocates a block of memory with a given allocator.

func CFAllocatorReallocate(CFAllocator!, UnsafeMutableRawPointer!, CFIndex, CFOptionFlags) -> UnsafeMutableRawPointer!

Reallocates memory using the specified allocator.

