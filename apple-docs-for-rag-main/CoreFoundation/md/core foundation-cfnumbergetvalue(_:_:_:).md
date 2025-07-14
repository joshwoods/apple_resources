

- Core Foundation
-  CFNumberGetValue(\_:\_:\_:) 

Function

# CFNumberGetValue(\_:\_:\_:)

Obtains the value of a CFNumber object cast to a specified type.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFNumberGetValue(
    _ number: CFNumber!,
    _ theType: CFNumberType,
    _ valuePtr: UnsafeMutableRawPointer!
) -> Bool
```

## Parameters 

`number`  

The CFNumber object to examine.

`theType`  

A constant that specifies the data type to return. See CFNumberType for a list of possible values.

`valuePtr`  

On return, contains the value of `number`.

## Return Value

`true` if the operation was successful, otherwise `false`.

## Discussion

If the argument type differs from the return type, and the conversion is lossy or the return value is out of range, then this function passes back an approximate value in `valuePtr` and returns `false`.

## See Also

### Getting Information About Numbers

func CFNumberGetByteSize(CFNumber!) -> CFIndex

Returns the number of bytes used by a CFNumber object to store its value.

func CFNumberGetType(CFNumber!) -> CFNumberType

Returns the type used by a CFNumber object to store its value.

func CFNumberIsFloatType(CFNumber!) -> Bool

Determines whether a CFNumber object contains a value stored as one of the defined floating point types.

