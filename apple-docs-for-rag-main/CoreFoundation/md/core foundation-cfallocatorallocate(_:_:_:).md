

- Core Foundation
-  CFAllocatorAllocate(\_:\_:\_:) 

Function

# CFAllocatorAllocate(\_:\_:\_:)

Allocates memory using the specified allocator.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFAllocatorAllocate(
    _ allocator: CFAllocator!,
    _ size: CFIndex,
    _ hint: CFOptionFlags
) -> UnsafeMutableRawPointer!
```

## Parameters 

`allocator`  

The allocator to use to allocate the memory. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`size`  

The size of the memory to allocate.

`hint`  

A bitfield containing flags that suggest how memory is to be allocated. `0` indicates no hints. No hints are currently defined, so only `0` should be passed for this value.

## Return Value

A pointer to the newly allocated memory.

## See Also

### Managing Memory with an Allocator

func CFAllocatorDeallocate(CFAllocator!, UnsafeMutableRawPointer!)

Deallocates a block of memory with a given allocator.

func CFAllocatorGetPreferredSizeForSize(CFAllocator!, CFIndex, CFOptionFlags) -> CFIndex

Obtains the number of bytes likely to be allocated upon a specific request.

func CFAllocatorReallocate(CFAllocator!, UnsafeMutableRawPointer!, CFIndex, CFOptionFlags) -> UnsafeMutableRawPointer!

Reallocates memory using the specified allocator.

