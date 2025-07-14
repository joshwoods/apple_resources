

- Core Foundation
-  CFArrayCreateCopy(\_:\_:) 

Function

# CFArrayCreateCopy(\_:\_:)

Creates a new immutable array with the values from another array.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFArrayCreateCopy(
    _ allocator: CFAllocator!,
    _ theArray: CFArray!
) -> CFArray!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new array and its storage for values. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`theArray`  

The array to copy.

## Return Value

A new CFArray object that contains the same values as `theArray`. Ownership follows The Create Rule.

## Discussion

The pointer values from `theArray` are copied into the new array; the values are also retained by the new array. The count of the new array is the same as `theArray`. The new array uses the same callbacks as `theArray`.

## See Also

### Creating an Array

func CFArrayCreate(CFAllocator!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!, CFIndex, UnsafePointer&lt;CFArrayCallBacks>!) -> CFArray!

Creates a new immutable array with the given values.

