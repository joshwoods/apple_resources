

- Core Foundation
-  CFBagCreateMutable(\_:\_:\_:) 

Function

# CFBagCreateMutable(\_:\_:\_:)

Creates a new empty mutable bag.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBagCreateMutable(
    _ allocator: CFAllocator!,
    _ capacity: CFIndex,
    _ callBacks: UnsafePointer!
) -> CFMutableBag!
```

## Parameters 

`allocator`  

The allocator object to use to allocate memory for the new bag and its storage for values. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`capacity`  

The maximum number of values that can be contained by the new bag. The bag starts empty and can grow to this number of values (and it can have less). If this parameter is `0`, the bag’s maximum capacity is not limited. This value must not be negative.

`callBacks`  

A pointer to a CFBagCallBacks structure initialized with the callbacks to use to retain, release, describe, and compare values in the bag. A copy of the contents of the callbacks structure is made, so that a pointer to a structure on the stack can be passed in or can be reused for multiple collection creations. This parameter may be `NULL`, which is treated as if a valid structure of version `0` with all fields `NULL` had been passed in.

If any of the fields are not valid pointers to functions of the correct type, or this parameter is not a valid pointer to a `CFBagCallBacks` structure, the behavior is undefined. If any value put into the collection is not one understood by one of the callback functions, the behavior when that callback function is used is undefined.

If the collection contains only CFType objects, then pass kCFTypeBagCallBacks as this parameter to use the default callback functions.

## Return Value

A new mutable bag, or `NULL` if there was a problem creating the object. Ownership follows the The Create Rule.

## Discussion

This function creates an new empty mutable bag to which you can add values using the CFBagAddValue(_:_:) function. The `capacity` parameter specifies the maximum number of values that the CFBag object can contain. If it is `0`, then there is no limit to the number of values that can be added (aside from constraints such as available memory).

## See Also

### Creating a Mutable Bag

func CFBagCreateMutableCopy(CFAllocator!, CFIndex, CFBag!) -> CFMutableBag!

Creates a new mutable bag with the values from another bag.

