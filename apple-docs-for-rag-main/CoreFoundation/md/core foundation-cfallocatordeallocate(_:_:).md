

- Core Foundation
-  CFAllocatorDeallocate(\_:\_:) 

Function

# CFAllocatorDeallocate(\_:\_:)

Deallocates a block of memory with a given allocator.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFAllocatorDeallocate(
    _ allocator: CFAllocator!,
    _ ptr: UnsafeMutableRawPointer!
)
```

## Parameters 

`allocator`  

The allocator that was used to allocate the block of memory pointed to by `ptr`.

`ptr`  

An untyped pointer to a block of memory to deallocate using `allocator`.

## Discussion

If the allocator does not specify a `deallocate` callback function, the memory is not deallocated.

### Special Considerations

You must use the same allocator to deallocate memory as was used to allocate it.

## See Also

### Managing Memory with an Allocator

func CFAllocatorAllocate(CFAllocator!, CFIndex, CFOptionFlags) -> UnsafeMutableRawPointer!

Allocates memory using the specified allocator.

func CFAllocatorGetPreferredSizeForSize(CFAllocator!, CFIndex, CFOptionFlags) -> CFIndex

Obtains the number of bytes likely to be allocated upon a specific request.

func CFAllocatorReallocate(CFAllocator!, UnsafeMutableRawPointer!, CFIndex, CFOptionFlags) -> UnsafeMutableRawPointer!

Reallocates memory using the specified allocator.

