

- Core Foundation
-  CFUUIDCreateWithBytes(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# CFUUIDCreateWithBytes(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:)

Creates a CFUUID object from raw UUID bytes.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFUUIDCreateWithBytes(
    _ alloc: CFAllocator!,
    _ byte0: UInt8,
    _ byte1: UInt8,
    _ byte2: UInt8,
    _ byte3: UInt8,
    _ byte4: UInt8,
    _ byte5: UInt8,
    _ byte6: UInt8,
    _ byte7: UInt8,
    _ byte8: UInt8,
    _ byte9: UInt8,
    _ byte10: UInt8,
    _ byte11: UInt8,
    _ byte12: UInt8,
    _ byte13: UInt8,
    _ byte14: UInt8,
    _ byte15: UInt8
) -> CFUUID!
```

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new CFUUID object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`byte0`  

Raw byte number `0`.

`byte1`  

Raw byte number `1`.

`byte2`  

Raw byte number `2`.

`byte3`  

Raw byte number `3`.

`byte4`  

Raw byte number `4`.

`byte5`  

Raw byte number `5`.

`byte6`  

Raw byte number `6`.

`byte7`  

Raw byte number `7`.

`byte8`  

Raw byte number `8`.

`byte9`  

Raw byte number `9`.

`byte10`  

Raw byte number `10`.

`byte11`  

Raw byte number `11`.

`byte12`  

Raw byte number `12`.

`byte13`  

Raw byte number `13`.

`byte14`  

Raw byte number `14`.

`byte15`  

Raw byte number `15`.

## Return Value

A new CFUUID object, or, if a CFUUID object of the same value already exists, the existing instance with its reference count incremented. Ownership follows the The Create Rule.

## Discussion

.

## See Also

### Creating CFUUID Objects

func CFUUIDCreate(CFAllocator!) -> CFUUID!

Creates a Universally Unique Identifier (UUID) object.

func CFUUIDCreateFromString(CFAllocator!, CFString!) -> CFUUID!

Creates a CFUUID object for a specified string.

func CFUUIDCreateFromUUIDBytes(CFAllocator!, CFUUIDBytes) -> CFUUID!

Creates a CFUUID object from raw UUID bytes.

