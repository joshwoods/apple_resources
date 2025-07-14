

- Core Foundation
-  CFUUIDCreateFromString(\_:\_:) 

Function

# CFUUIDCreateFromString(\_:\_:)

Creates a CFUUID object for a specified string.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFUUIDCreateFromString(
    _ alloc: CFAllocator!,
    _ uuidStr: CFString!
) -> CFUUID!
```

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new CFUUID object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`uuidStr`  

A string containing a UUID. The standard format for UUIDs represented in ASCII is a string punctuated by hyphens, for example `68753A44-4D6F-1226-9C60-0050E4C00067`.

## Return Value

A new CFUUID object, or if a CFUUID object of the same value already exists, the existing instance with its reference count incremented. Ownership follows the The Create Rule.

## See Also

### Creating CFUUID Objects

func CFUUIDCreate(CFAllocator!) -> CFUUID!

Creates a Universally Unique Identifier (UUID) object.

func CFUUIDCreateFromUUIDBytes(CFAllocator!, CFUUIDBytes) -> CFUUID!

Creates a CFUUID object from raw UUID bytes.

func CFUUIDCreateWithBytes(CFAllocator!, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8) -> CFUUID!

Creates a CFUUID object from raw UUID bytes.

