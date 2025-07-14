

- Core Foundation
-  CFBagCreate(\_:\_:\_:\_:) 

Function

# CFBagCreate(\_:\_:\_:\_:)

Creates an immutable bag containing specified values.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBagCreate(
    _ allocator: CFAllocator!,
    _ values: UnsafeMutablePointer!,
    _ numValues: CFIndex,
    _ callBacks: UnsafePointer!
) -> CFBag!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new bag and its storage for values. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`values`  

A C array of the pointer-sized values to be in the new bag. This parameter may be `NULL` if the `numValues` parameter is 0. The C array is not changed or freed by this function. `values` must be a valid pointer to a C array of at least `numValues` elements.

`numValues`  

The number of values to copy from the `values` C array in the new CFBag object. If the number is negative or is greater than the actual number of values, the behavior is undefined.

`callBacks`  

A pointer to a CFBagCallBacks structure initialized with the callbacks to use to retain, release, describe, and compare values in the bag. A copy of the contents of the callbacks structure is made, so that a pointer to a structure on the stack can be passed in or can be reused for multiple collection creations. This parameter may be `NULL`, which is treated as if a valid structure of version 0 with all fields `NULL` had been passed in. Otherwise, if any of the fields are not valid pointers to functions of the correct type, or this parameter is not a valid pointer to a CFBagCallBacks structure, the behavior is undefined. If any value put into the collection is not one understood by one of the callback functions, the behavior when that callback function is used is undefined. If the collection contains CFType objects only, then pass kCFTypeBagCallBacks as this parameter to use the default callback functions.

## Return Value

A new bag, or `NULL` if there was a problem creating the object. Ownership follows the The Create Rule.

## See Also

### Creating a Bag

func CFBagCreateCopy(CFAllocator!, CFBag!) -> CFBag!

Creates an immutable bag with the values of another bag.

