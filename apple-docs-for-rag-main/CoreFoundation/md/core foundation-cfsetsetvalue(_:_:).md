

- Core Foundation
-  CFSetSetValue(\_:\_:) 

Function

# CFSetSetValue(\_:\_:)

Sets a value in a CFMutableSet object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFSetSetValue(
    _ theSet: CFMutableSet!,
    _ value: UnsafeRawPointer!
)
```

## Parameters 

`theSet`  

The set to modify.

`value`  

The value to be set in `theSet`. If this value already exists in `theSet`, it is replaced. You may pass the value itself instead of a pointer to it if the value is pointer-size or less. If `theSet` is fixed-size and setting the value would increase its size beyond its capacity, the behavior is undefined.

## Discussion

Depending on the implementation of the equal callback specified when creating `theSet`, the value that is replaced by `value` may not have the same pointer equality.

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

func CFSetReplaceValue(CFMutableSet!, UnsafeRawPointer!)

Replaces a value in a CFMutableSet object.

