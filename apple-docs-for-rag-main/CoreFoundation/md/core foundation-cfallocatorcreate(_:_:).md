

- Core Foundation
-  CFAllocatorCreate(\_:\_:) 

Function

# CFAllocatorCreate(\_:\_:)

Creates an allocator object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFAllocatorCreate(
    _ allocator: CFAllocator!,
    _ context: UnsafeMutablePointer!
) -> Unmanaged!
```

## Parameters 

`allocator`  

The existing allocator to use to allocate memory for the new allocator. Pass the kCFAllocatorUseContext constant for this parameter to allocate memory using the appropriate function callback specified in the `context` parameter. Pass `NULL` or kCFAllocatorDefault to allocate memory for the new allocator using the default allocator.

`context`  

A structure of type CFAllocatorContext. The fields of this structure hold (among other things) function pointers to callbacks used for allocating, reallocating, and deallocating memory.

## Return Value

The new allocator object, or `NULL` if there was a problem allocating memory. Ownership follows the The Create Rule.

## Discussion

You use this function to create custom allocators which you can then pass into various Core Foundation object-creation functions. You must implement a function callback that allocates memory and assign it to the `allocate` field of this structure. You typically also implement deallocate, reallocate, and preferred-size callbacks.

