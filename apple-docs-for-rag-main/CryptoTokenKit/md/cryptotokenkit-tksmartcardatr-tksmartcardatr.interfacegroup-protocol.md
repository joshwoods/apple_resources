

- CryptoTokenKit
- TKSmartCardATR
- TKSmartCardATR.InterfaceGroup
-  protocol 

Instance Property

# protocol

The protocol for this group.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var `protocol`: NSNumber? { get }
```

## Discussion

This property returns an `NSNumber` object containing an `NSUInteger` value corresponding to a member of the TKSmartCardProtocol enumeration.

This property is `nil` for the first interface group (global), as it has no assigned protocol.

## See Also

### Accessing Interface Group Protocol and Bytes

var ta: NSNumber?

The TA interface byte of ATR group, or `nil` if TA is not present.

var tb: NSNumber?

The TB interface byte of ATR group, or `nil` if TB is not present.

var tc: NSNumber?

The TC interface byte of ATR group, or `nil` if TC is not present.

