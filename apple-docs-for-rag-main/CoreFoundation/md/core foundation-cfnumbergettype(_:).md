

- Core Foundation
-  CFNumberGetType(\_:) 

Function

# CFNumberGetType(\_:)

Returns the type used by a CFNumber object to store its value.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFNumberGetType(_ number: CFNumber!) -> CFNumberType
```

## Parameters 

`number`  

The CFNumber object to examine.

## Return Value

A constant that indicates the data type of the value contained in `number`. See CFNumberType for a list of possible values.

## Discussion

The type specified in the call to CFNumberCreate(_:_:_:) is not necessarily preserved when a new CFNumber object is created—it uses whatever internal storage type the creation function deems appropriate.

## See Also

### Getting Information About Numbers

func CFNumberGetByteSize(CFNumber!) -> CFIndex

Returns the number of bytes used by a CFNumber object to store its value.

func CFNumberGetValue(CFNumber!, CFNumberType, UnsafeMutableRawPointer!) -> Bool

Obtains the value of a CFNumber object cast to a specified type.

func CFNumberIsFloatType(CFNumber!) -> Bool

Determines whether a CFNumber object contains a value stored as one of the defined floating point types.

