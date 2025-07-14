

- CryptoTokenKit
- TKSmartCardSlot
-  atr 

Instance Property

# atr

The ATR (Answer to Reset) of the inserted Smart Card, or `nil` if no Smart Card is inserted or the inserted Smart Card is mute.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var atr: TKSmartCardATR? { get }
```

## See Also

### Reading the Answer to Reset

class TKSmartCardATR

A parsed ATR (Answer To Reset) message from a Smart Card.

