

- CryptoTokenKit
- TKSmartCard
-  context 

Instance Property

# context

User-specified information. This property is automatically set to `nil` if the Smart Card is removed or another `TKSmartCard` object begins a session.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var context: Any? { get set }
```

## See Also

### Configuring the Smart Card

var slot: TKSmartCardSlot

The slot in which the Smart Card is inserted.

var isValid: Bool

Whether the Smart Card is valid and accessible from its slot.

var isSensitive: Bool

Whether sessions established for the Smart Card should be considered sensitive. false by default.

