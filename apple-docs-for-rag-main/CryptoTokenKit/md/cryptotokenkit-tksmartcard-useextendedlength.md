

- CryptoTokenKit
- TKSmartCard
-  useExtendedLength 

Instance Property

# useExtendedLength

Whether to use extended length APDU.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var useExtendedLength: Bool { get set }
```

## Discussion

By default, this property is set to true when the Smart Card slot supports transmitting extended length commands, and the ATR announces that extended length APDU is supported.

## See Also

### Configuring APDU Behavior

var cla: UInt8

The CLA byte used for APDU transmission. `0x00` by default.

var useCommandChaining: Bool

Whether to use command chaining of APDU with a data field longer than 255 bytes.

