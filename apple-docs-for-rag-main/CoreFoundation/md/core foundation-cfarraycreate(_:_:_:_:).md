

- Core Foundation
-  CFArrayCreate(\_:\_:\_:\_:) 

Function

# CFArrayCreate(\_:\_:\_:\_:)

Creates a new immutable array with the given values.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFArrayCreate(
    _ allocator: CFAllocator!,
    _ values: UnsafeMutablePointer!,
    _ numValues: CFIndex,
    _ callBacks: UnsafePointer!
) -> CFArray!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new array and its storage for values. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`values`  

A C array of the pointer-sized values to be in the new array. The values in the new array are ordered in the same order in which they appear in this C array. This value may be `NULL` if `numValues` is `0`. This C array is not changed or freed by this function. If `values` is not a valid pointer to a C array of at least `numValues` elements, the behavior is undefined.

`numValues`  

The number of values to copy from the values C array into the new array. This number will be the count of the new array—it must not be negative or greater than the number of elements in `values`.

`callBacks`  

A pointer to a CFArrayCallBacks structure initialized with the callbacks for the array to use on each value in the collection. The retain callback is used within this function, for example, to retain all of the new values from the values C array. A copy of the contents of the callbacks structure is made, so that a pointer to a structure on the stack can be passed in or can be reused for multiple collection creations.

This value may be `NULL`, which is treated as if a valid structure of version `0` with all fields `NULL` had been passed in. Otherwise, if any of the fields are not valid pointers to functions of the correct type, or this value is not a valid pointer to a CFArrayCallBacks structure, the behavior is undefined. If any value put into the collection is not one understood by one of the callback functions, the behavior when that callback function is used is undefined.

If the collection contains only CFType objects, then pass a pointer to kCFTypeArrayCallBacks (`&kCFTypeArrayCallBacks`) to use the default callback functions.

## Return Value

A new immutable array containing `numValues` from `values`, or `NULL` if there was a problem creating the object. Ownership follows The Create Rule.

## See Also

### Creating an Array

func CFArrayCreateCopy(CFAllocator!, CFArray!) -> CFArray!

Creates a new immutable array with the values from another array.

