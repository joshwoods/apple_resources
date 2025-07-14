

- CryptoTokenKit
- TKSmartCard
-  useCommandChaining 

Instance Property

# useCommandChaining

Whether to use command chaining of APDU with a data field longer than 255 bytes.

iOSiPadOSMac Catalyst 13.1+macOS 10.12+tvOSvisionOSwatchOS

``` source
var useCommandChaining: Bool { get set }
```

## Discussion

By default, this property is set to true when the Smart Card ATR announces that command chaining is supported.

## See Also

### Configuring APDU Behavior

var cla: UInt8

The CLA byte used for APDU transmission. `0x00` by default.

var useExtendedLength: Bool

Whether to use extended length APDU.

