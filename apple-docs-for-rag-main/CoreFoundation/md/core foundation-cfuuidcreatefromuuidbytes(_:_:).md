

- Core Foundation
-  CFUUIDCreateFromUUIDBytes(\_:\_:) 

Function

# CFUUIDCreateFromUUIDBytes(\_:\_:)

Creates a CFUUID object from raw UUID bytes.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFUUIDCreateFromUUIDBytes(
    _ alloc: CFAllocator!,
    _ bytes: CFUUIDBytes
) -> CFUUID!
```

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new CFUUID object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`bytes`  

Raw UUID bytes to use to create the CFUUID object.

## Return Value

A new CFUUID object. Ownership follows the The Create Rule.

## See Also

### Creating CFUUID Objects

func CFUUIDCreate(CFAllocator!) -> CFUUID!

Creates a Universally Unique Identifier (UUID) object.

func CFUUIDCreateFromString(CFAllocator!, CFString!) -> CFUUID!

Creates a CFUUID object for a specified string.

func CFUUIDCreateWithBytes(CFAllocator!, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8) -> CFUUID!

Creates a CFUUID object from raw UUID bytes.

