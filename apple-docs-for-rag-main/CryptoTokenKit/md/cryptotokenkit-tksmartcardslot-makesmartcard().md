

- CryptoTokenKit
- TKSmartCardSlot
-  makeSmartCard() 

Instance Method

# makeSmartCard()

Creates a new TKSmartCard object representing the currently inserted Smart Card.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func makeSmartCard() -> TKSmartCard?
```

## Return Value

A new TKSmartCard object, or `nil` if no Smart Card is currently inserted.

## Discussion

You can create multiple instances of `TKSmartCard` that represent the same Smart Card. Exclusivity of data transfer is handled by sessions on the individual `TKSmartCard` objects.

