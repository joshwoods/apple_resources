

- Core Foundation
-  CFAllocatorReallocate(\_:\_:\_:\_:) 

Function

# CFAllocatorReallocate(\_:\_:\_:\_:)

Reallocates memory using the specified allocator.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFAllocatorReallocate(
    _ allocator: CFAllocator!,
    _ ptr: UnsafeMutableRawPointer!,
    _ newsize: CFIndex,
    _ hint: CFOptionFlags
) -> UnsafeMutableRawPointer!
```

## Parameters 

`allocator`  

The allocator to use for reallocating memory. Pass `NULL` to request the default allocator.

`ptr`  

An untyped pointer to a block of memory to reallocate to a new size. If `ptr` is `NULL` and `newsize` is greater than 0, memory is allocated (using the `allocate` function callback of the allocator’s context). If `ptr` is `NULL` and `newsize` is 0, the result is `NULL`.

`newsize`  

The number of bytes to allocate. If you pass `0` and the `ptr` parameter is non-`NULL`, the block of memory that `ptr` points to is typically deallocated. If you pass 0 for this parameter and the `ptr` parameter is `NULL`, nothing happens and the result returned is `NULL`.

`hint`  

A bitfield of type `CFOptionsFlags`. Pass flags to the allocator that suggest how memory is to be allocated. Zero indicates no hints. No hints are currently defined, only `0` should be passed for this argument.

## Discussion

The `CFAllocatorReallocate` function’s primary purpose is to reallocate a block of memory to a new (and usually larger) size. However, based on the values passed in certain of the parameters, this function can also allocate memory afresh or deallocate a given block of memory. The following summarizes the semantic combinations:

- If the `ptr` parameter is non- `NULL` and the `newsize` parameter is greater than `0`, the behavior is to reallocate.

- If the `ptr` parameter is `NULL` and the `newsize` parameter is greater than `0`, the behavior is to allocate.

- If the `ptr` parameter is non- `NULL` and the `newsize` parameter is `0`, the behavior is to deallocate.

The result of the `CFAllocatorReallocate` function is either an untyped pointer to a block of memory or `NULL`. A `NULL` result indicates either a failure to allocate memory or some other outcome, the precise interpretation of which is determined by the values of certain parameters and the presence or absence of callbacks in the allocator context. To summarize, a `NULL` result can mean one of the following:

- An error occurred in the attempt to allocate memory, such as insufficient free space.

- No `allocate`, `reallocate`, or `deallocate` function callback (depending on parameters) was defined in the allocator context.

- The semantic operation is “deallocate” (that is, there is no need to return anything).

- The `ptr` parameter is `NULL` and the requested size is 0.

## See Also

### Managing Memory with an Allocator

func CFAllocatorAllocate(CFAllocator!, CFIndex, CFOptionFlags) -> UnsafeMutableRawPointer!

Allocates memory using the specified allocator.

func CFAllocatorDeallocate(CFAllocator!, UnsafeMutableRawPointer!)

Deallocates a block of memory with a given allocator.

func CFAllocatorGetPreferredSizeForSize(CFAllocator!, CFIndex, CFOptionFlags) -> CFIndex

Obtains the number of bytes likely to be allocated upon a specific request.

