

- Core Foundation
-  CFBagCreateMutableCopy(\_:\_:\_:) 

Function

# CFBagCreateMutableCopy(\_:\_:\_:)

Creates a new mutable bag with the values from another bag.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBagCreateMutableCopy(
    _ allocator: CFAllocator!,
    _ capacity: CFIndex,
    _ theBag: CFBag!
) -> CFMutableBag!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new bag and its storage for values. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`capacity`  

The maximum number of values that can be contained by the new bag. The bag starts with the same count as `theBag`, and can grow to this number of values (and it can have less). If this value is `0`, the bag’s maximum capacity is not limited. This value must be greater than or equal to the count of `theBag`, and must not be negative.

`theBag`  

The bag to copy. The pointer values from `theBag` are copied into the new bag. However, the values are also retained by the new bag. The count of the new bag is the same as the count of `theBag`. The new bag uses the same callbacks as `theBag`.

## Return Value

A new mutable bag that contains the same values as `theBag`. Ownership follows the The Create Rule.

## See Also

### Creating a Mutable Bag

func CFBagCreateMutable(CFAllocator!, CFIndex, UnsafePointer&lt;CFBagCallBacks>!) -> CFMutableBag!

Creates a new empty mutable bag.

