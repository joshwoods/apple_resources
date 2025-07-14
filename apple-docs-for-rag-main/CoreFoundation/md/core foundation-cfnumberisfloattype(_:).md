

- Core Foundation
-  CFNumberIsFloatType(\_:) 

Function

# CFNumberIsFloatType(\_:)

Determines whether a CFNumber object contains a value stored as one of the defined floating point types.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFNumberIsFloatType(_ number: CFNumber!) -> Bool
```

## Parameters 

`number`  

The CFNumber object to examine.

## Return Value

`true` if `number`’s value is one of the defined floating point types, otherwise `false`. The valid floating point types are listed in CFNumberType.

## See Also

### Getting Information About Numbers

func CFNumberGetByteSize(CFNumber!) -> CFIndex

Returns the number of bytes used by a CFNumber object to store its value.

func CFNumberGetType(CFNumber!) -> CFNumberType

Returns the type used by a CFNumber object to store its value.

func CFNumberGetValue(CFNumber!, CFNumberType, UnsafeMutableRawPointer!) -> Bool

Obtains the value of a CFNumber object cast to a specified type.

