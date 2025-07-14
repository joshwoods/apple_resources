

- Core Foundation
-  CFSetCreate(\_:\_:\_:\_:) 

Function

# CFSetCreate(\_:\_:\_:\_:)

Creates an immutable CFSet object containing supplied values.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFSetCreate(
    _ allocator: CFAllocator!,
    _ values: UnsafeMutablePointer!,
    _ numValues: CFIndex,
    _ callBacks: UnsafePointer!
) -> CFSet!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new set and its storage for values. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`values`  

A C array of the pointer-sized values to be in the new set. This parameter may be `NULL` if the `numValues` parameter is 0. The C array is not changed or freed by this function. `values` must be a pointer to a C array of at least `numValues` elements.

`numValues`  

The number of values to copy from the `values` C array in the new set.

`callBacks`  

A pointer to a CFSetCallBacks structure initialized with the callbacks to use to retain, release, describe, and compare values in the collection. A copy of the contents of the callbacks structure is made, so that a pointer to a structure on the stack can be passed in or can be reused for multiple collection creations.

This value may be `NULL`, which is treated as a valid structure of version `0` with all fields `NULL`. If the collection contains only CFType objects, then pass kCFTypeSetCallBacks to use the default callback functions.

## Return Value

A new immutable set, or `NULL` if there was a problem creating the object. Ownership follows the The Create Rule.

## Discussion

If any value put into the collection is not one understood by one of the callback functions, the behavior when that callback function is used is undefined.

## See Also

### Creating Sets

func CFSetCreateCopy(CFAllocator!, CFSet!) -> CFSet!

Creates an immutable set containing the values of an existing set.

