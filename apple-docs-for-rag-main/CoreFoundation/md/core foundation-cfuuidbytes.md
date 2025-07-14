

- Core Foundation
-  CFUUIDBytes 

Structure

# CFUUIDBytes

A 128-bit struct that represents a UUID as raw bytes.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CFUUIDBytes
```

## Overview

This structure can be obtained from a CFUUID object using the CFUUIDGetUUIDBytes(_:) function. This structure can be passed to functions that expect a raw UUID.

## Topics

### Initializers

init()

init(byte0: UInt8, byte1: UInt8, byte2: UInt8, byte3: UInt8, byte4: UInt8, byte5: UInt8, byte6: UInt8, byte7: UInt8, byte8: UInt8, byte9: UInt8, byte10: UInt8, byte11: UInt8, byte12: UInt8, byte13: UInt8, byte14: UInt8, byte15: UInt8)

### Instance Properties

var byte0: UInt8

The first byte.

var byte1: UInt8

The second byte.

var byte10: UInt8

The eleventh byte.

var byte11: UInt8

The twelfth byte.

var byte12: UInt8

The thirteenth byte.

var byte13: UInt8

The fourteenth byte.

var byte14: UInt8

The fifteenth byte.

var byte15: UInt8

The sixteenth byte.

var byte2: UInt8

The third byte.

var byte3: UInt8

The fourth byte.

var byte4: UInt8

The fifth byte.

var byte5: UInt8

The sixth byte.

var byte6: UInt8

The seventh byte.

var byte7: UInt8

The eighth byte.

var byte8: UInt8

The ninth byte.

var byte9: UInt8

The tenth byte.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

