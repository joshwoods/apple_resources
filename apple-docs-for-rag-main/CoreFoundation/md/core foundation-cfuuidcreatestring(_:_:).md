

- Core Foundation
-  CFUUIDCreateString(\_:\_:) 

Function

# CFUUIDCreateString(\_:\_:)

Returns the string representation of a specified CFUUID object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFUUIDCreateString(
    _ alloc: CFAllocator!,
    _ uuid: CFUUID!
) -> CFString!
```

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new string. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`uuid`  

The CFUUID object whose string representation to obtain.

## Return Value

The string representation of `uuid`. Ownership follows the The Create Rule.

## See Also

### Getting Information About CFUUID Objects

func CFUUIDGetConstantUUIDWithBytes(CFAllocator!, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8) -> CFUUID!

Returns a CFUUID object from raw UUID bytes.

func CFUUIDGetUUIDBytes(CFUUID!) -> CFUUIDBytes

Returns the value of a UUID object as raw bytes.

