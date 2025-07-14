

- CryptoTokenKit
- TKSmartCardATR
-  TKSmartCardATR.InterfaceGroup 

Class

# TKSmartCardATR.InterfaceGroup

A single interface-bytes group for a Smart Card ATR (Answer to Reset).

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
class InterfaceGroup
```

## Overview

You access instances of this class by calling the interfaceGroup(at:) and interfaceGroup(for:) methods on an TKSmartCardATR object.

## Topics

### Accessing Interface Group Protocol and Bytes

var `protocol`: NSNumber?

The protocol for this group.

var ta: NSNumber?

The TA interface byte of ATR group, or `nil` if TA is not present.

var tb: NSNumber?

The TB interface byte of ATR group, or `nil` if TB is not present.

var tc: NSNumber?

The TC interface byte of ATR group, or `nil` if TC is not present.

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

### Retrieving Interface Groups

func interfaceGroup(at: Int) -> TKSmartCardATR.InterfaceGroup?

Returns the interface group at the specified index.

func interfaceGroup(for: TKSmartCardProtocol) -> TKSmartCardATR.InterfaceGroup?

Returns the interface group with the specified protocol.

