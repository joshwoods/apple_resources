

- Core Foundation
-  CFSetAddValue(\_:\_:) 

Function

# CFSetAddValue(\_:\_:)

Adds a value to a CFMutableSet object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFSetAddValue(
    _ theSet: CFMutableSet!,
    _ value: UnsafeRawPointer!
)
```

## Parameters 

`theSet`  

The set to modify.

`value`  

A CFType object or a pointer value to add to `theSet` (or the value itself, if it fits into the size of a pointer).

`value` is retained by `theSet` using the retain callback provided when `theSet` was created. If `value` is not of the type expected by the retain callback, the behavior is undefined. If `value` already exists in the collection, this function returns without doing anything.

## See Also

### CFMutableSet Miscellaneous Functions

func CFSetCreateMutable(CFAllocator!, CFIndex, UnsafePointer&lt;CFSetCallBacks>!) -> CFMutableSet!

Creates an empty CFMutableSet object.

func CFSetCreateMutableCopy(CFAllocator!, CFIndex, CFSet!) -> CFMutableSet!

Creates a new mutable set with the values from another set.

func CFSetRemoveAllValues(CFMutableSet!)

Removes all values from a CFMutableSet object.

func CFSetRemoveValue(CFMutableSet!, UnsafeRawPointer!)

Removes a value from a CFMutableSet object.

func CFSetReplaceValue(CFMutableSet!, UnsafeRawPointer!)

Replaces a value in a CFMutableSet object.

func CFSetSetValue(CFMutableSet!, UnsafeRawPointer!)

Sets a value in a CFMutableSet object.

