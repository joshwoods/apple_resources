

- Core Foundation
-  CFBagCreateCopy(\_:\_:) 

Function

# CFBagCreateCopy(\_:\_:)

Creates an immutable bag with the values of another bag.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBagCreateCopy(
    _ allocator: CFAllocator!,
    _ theBag: CFBag!
) -> CFBag!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new bag and its storage for values. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`theBag`  

The bag to copy. The pointer values from `theBag` are copied into the new bag. However, the values are also retained by the new bag. The count of the new bag is the same as the count of `theBag`. The new bag uses the same callbacks as `theBag`.

## Return Value

A new bag that contains the same values as `theBag`, or `NULL` if there was a problem creating the object. Ownership follows the The Create Rule.

## See Also

### Creating a Bag

func CFBagCreate(CFAllocator!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!, CFIndex, UnsafePointer&lt;CFBagCallBacks>!) -> CFBag!

Creates an immutable bag containing specified values.

