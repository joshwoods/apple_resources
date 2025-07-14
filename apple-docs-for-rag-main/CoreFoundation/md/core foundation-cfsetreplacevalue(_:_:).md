

- Core Foundation
-  CFSetReplaceValue(\_:\_:) 

Function

# CFSetReplaceValue(\_:\_:)

Replaces a value in a CFMutableSet object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFSetReplaceValue(
    _ theSet: CFMutableSet!,
    _ value: UnsafeRawPointer!
)
```

## Parameters 

`theSet`  

The set to modify.

`value`  

The value to replace in `theSet`. If this value does not already exist in `theSet`, the function does nothing. You may pass the value itself instead of a pointer if it is pointer-size or less. The equal callback provided when `theSet` was created is used to compare. If the equal callback was `NULL`, pointer equality (in C, ==) is used. If `value`, or any other value in `theSet`, is not understood by the equal callback, the behavior is undefined.

## See Also

### CFMutableSet Miscellaneous Functions

func CFSetAddValue(CFMutableSet!, UnsafeRawPointer!)

Adds a value to a CFMutableSet object.

func CFSetCreateMutable(CFAllocator!, CFIndex, UnsafePointer&lt;CFSetCallBacks>!) -> CFMutableSet!

Creates an empty CFMutableSet object.

func CFSetCreateMutableCopy(CFAllocator!, CFIndex, CFSet!) -> CFMutableSet!

Creates a new mutable set with the values from another set.

func CFSetRemoveAllValues(CFMutableSet!)

Removes all values from a CFMutableSet object.

func CFSetRemoveValue(CFMutableSet!, UnsafeRawPointer!)

Removes a value from a CFMutableSet object.

func CFSetSetValue(CFMutableSet!, UnsafeRawPointer!)

Sets a value in a CFMutableSet object.

