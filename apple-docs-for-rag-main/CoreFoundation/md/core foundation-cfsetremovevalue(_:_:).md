

- Core Foundation
-  CFSetRemoveValue(\_:\_:) 

Function

# CFSetRemoveValue(\_:\_:)

Removes a value from a CFMutableSet object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFSetRemoveValue(
    _ theSet: CFMutableSet!,
    _ value: UnsafeRawPointer!
)
```

## Parameters 

`theSet`  

The set to modify.

`value`  

The value to remove from `theSet`.

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

func CFSetReplaceValue(CFMutableSet!, UnsafeRawPointer!)

Replaces a value in a CFMutableSet object.

func CFSetSetValue(CFMutableSet!, UnsafeRawPointer!)

Sets a value in a CFMutableSet object.

