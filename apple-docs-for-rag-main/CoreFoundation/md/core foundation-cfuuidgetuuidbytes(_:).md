

- Core Foundation
-  CFUUIDGetUUIDBytes(\_:) 

Function

# CFUUIDGetUUIDBytes(\_:)

Returns the value of a UUID object as raw bytes.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFUUIDGetUUIDBytes(_ uuid: CFUUID!) -> CFUUIDBytes
```

## Parameters 

`uuid`  

The CFUUID object to examine.

## Return Value

The value of `uuid` represented as raw bytes.

## See Also

### Getting Information About CFUUID Objects

func CFUUIDCreateString(CFAllocator!, CFUUID!) -> CFString!

Returns the string representation of a specified CFUUID object.

func CFUUIDGetConstantUUIDWithBytes(CFAllocator!, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8) -> CFUUID!

Returns a CFUUID object from raw UUID bytes.

