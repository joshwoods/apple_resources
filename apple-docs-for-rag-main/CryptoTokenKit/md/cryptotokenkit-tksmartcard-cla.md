

- CryptoTokenKit
- TKSmartCard
-  cla 

Instance Property

# cla

The CLA byte used for APDU transmission. `0x00` by default.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var cla: UInt8 { get set }
```

## See Also

### Configuring APDU Behavior

var useExtendedLength: Bool

Whether to use extended length APDU.

var useCommandChaining: Bool

Whether to use command chaining of APDU with a data field longer than 255 bytes.

