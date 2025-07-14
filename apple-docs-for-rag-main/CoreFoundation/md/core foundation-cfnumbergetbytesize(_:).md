

- Core Foundation
-  CFNumberGetByteSize(\_:) 

Function

# CFNumberGetByteSize(\_:)

Returns the number of bytes used by a CFNumber object to store its value.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFNumberGetByteSize(_ number: CFNumber!) -> CFIndex
```

## Parameters 

`number`  

The CFNumber object to examine.

## Return Value

The size in bytes of the value contained in `number`.

## Discussion

Because a CFNumber object might store a value using a type different from that of the original value with which it was created, this function may return a size different from the size of the original value’s type.

## See Also

### Getting Information About Numbers

func CFNumberGetType(CFNumber!) -> CFNumberType

Returns the type used by a CFNumber object to store its value.

func CFNumberGetValue(CFNumber!, CFNumberType, UnsafeMutableRawPointer!) -> Bool

Obtains the value of a CFNumber object cast to a specified type.

func CFNumberIsFloatType(CFNumber!) -> Bool

Determines whether a CFNumber object contains a value stored as one of the defined floating point types.

