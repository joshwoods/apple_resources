

- Core Foundation
-  CFUUIDCreate(\_:) 

Function

# CFUUIDCreate(\_:)

Creates a Universally Unique Identifier (UUID) object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFUUIDCreate(_ alloc: CFAllocator!) -> CFUUID!
```

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new CFUUID object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

## Return Value

A new CFUUID object. Ownership follows the The Create Rule.

## See Also

### Creating CFUUID Objects

func CFUUIDCreateFromString(CFAllocator!, CFString!) -> CFUUID!

Creates a CFUUID object for a specified string.

func CFUUIDCreateFromUUIDBytes(CFAllocator!, CFUUIDBytes) -> CFUUID!

Creates a CFUUID object from raw UUID bytes.

func CFUUIDCreateWithBytes(CFAllocator!, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8) -> CFUUID!

Creates a CFUUID object from raw UUID bytes.

