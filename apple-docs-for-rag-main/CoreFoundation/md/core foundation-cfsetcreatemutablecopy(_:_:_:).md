

- Core Foundation
-  CFSetCreateMutableCopy(\_:\_:\_:) 

Function

# CFSetCreateMutableCopy(\_:\_:\_:)

Creates a new mutable set with the values from another set.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFSetCreateMutableCopy(
    _ allocator: CFAllocator!,
    _ capacity: CFIndex,
    _ theSet: CFSet!
) -> CFMutableSet!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new set and its storage for values. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`capacity`  

The maximum number of values that can be contained by the new set. The set starts with the same number of values as `theSet` and can grow to this number of values (and it can have less).

Pass `0` to specify that the maximum capacity is not limited. If non-`0`, `capacity` must be greater than or equal to the count of `theSet`.

`theSet`  

The set to copy. The pointer values from `theSet` are copied into the new set. The values are also retained by the new set. The count of the new set is the same as the count of `theSet`. The new set uses the same callbacks as `theSet`.

## Return Value

A new mutable set that contains the same values as `theSet`. Ownership follows the The Create Rule.

## See Also

### CFMutableSet Miscellaneous Functions

func CFSetAddValue(CFMutableSet!, UnsafeRawPointer!)

Adds a value to a CFMutableSet object.

func CFSetCreateMutable(CFAllocator!, CFIndex, UnsafePointer&lt;CFSetCallBacks>!) -> CFMutableSet!

Creates an empty CFMutableSet object.

func CFSetRemoveAllValues(CFMutableSet!)

Removes all values from a CFMutableSet object.

func CFSetRemoveValue(CFMutableSet!, UnsafeRawPointer!)

Removes a value from a CFMutableSet object.

func CFSetReplaceValue(CFMutableSet!, UnsafeRawPointer!)

Replaces a value in a CFMutableSet object.

func CFSetSetValue(CFMutableSet!, UnsafeRawPointer!)

Sets a value in a CFMutableSet object.

