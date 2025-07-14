

- CryptoTokenKit
-  TKSmartCardATR 

Class

# TKSmartCardATR

A parsed ATR (Answer To Reset) message from a Smart Card.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class TKSmartCardATR
```

## Overview

This class declares a programmatic interface to parsing an ATR from data or a byte stream, and accessing the individual parts.

Note

The TKSmartCardATR class parses ATR messages according to the ISO/IEC 7816-3 specification.

## Topics

### Creating a Smart Card ATR

init?(bytes: Data)

Initializes a `TKSmartCardATR` object from a provided data object.

init?(source: () -> Int32)

Initializes a `TKSmartCardATR` object from a provided data source.

### Accessing ATR Attributes

var protocols: [NSNumber]

An array of protocols indicated in the ATR

var bytes: Data

The ATR message data.

var historicalBytes: Data

The ATR historical bytes, not including interface bytes or the TCK (check byte).

var historicalRecords: [TKCompactTLVRecord]?

A list of compact TLV records parsed from historical bytes.

### Retrieving Interface Groups

func interfaceGroup(at: Int) -> TKSmartCardATR.InterfaceGroup?

Returns the interface group at the specified index.

func interfaceGroup(for: TKSmartCardProtocol) -> TKSmartCardATR.InterfaceGroup?

Returns the interface group with the specified protocol.

class InterfaceGroup

A single interface-bytes group for a Smart Card ATR (Answer to Reset).

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Reading the Answer to Reset

var atr: TKSmartCardATR?

The ATR (Answer to Reset) of the inserted Smart Card, or `nil` if no Smart Card is inserted or the inserted Smart Card is mute.

