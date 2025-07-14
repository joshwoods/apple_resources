

- Core Foundation
-  CFTreeCreate(\_:\_:) 

Function

# CFTreeCreate(\_:\_:)

Creates a new CFTree object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFTreeCreate(
    _ allocator: CFAllocator!,
    _ context: UnsafePointer!
) -> CFTree!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new tree. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`context`  

The CFTreeContext structure to be copied and used as the context of the new tree. The information pointer will be retained by the tree if a retain function is provided. If this value is not a valid C pointer to a CFTreeContext structure-sized block of storage, the result is undefined. If the version number of the storage is not a valid CFTreeContext version number, the result is undefined.

## Return Value

A new CFTree object. Ownership follows the The Create Rule.

