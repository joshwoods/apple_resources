

- Core Foundation
-  CFSetCreateCopy(\_:\_:) 

Function

# CFSetCreateCopy(\_:\_:)

Creates an immutable set containing the values of an existing set.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFSetCreateCopy(
    _ allocator: CFAllocator!,
    _ theSet: CFSet!
) -> CFSet!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new set and its storage for values. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`theSet`  

The set to copy.

## Return Value

A new set that contains the same values as `theSet`, or `NULL` if there was a problem creating the object. Ownership follows the The Create Rule.

## Discussion

The pointer values from `theSet` are copied into the new set, and the values are retained by the new set. The count of the new set is the same as the count of `theSet`. The new set uses the same callbacks as `theSet`.

## See Also

### Creating Sets

func CFSetCreate(CFAllocator!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!, CFIndex, UnsafePointer&lt;CFSetCallBacks>!) -> CFSet!

Creates an immutable CFSet object containing supplied values.

