

- CryptoTokenKit
- TKSmartCard
-  isSensitive 

Instance Property

# isSensitive

Whether sessions established for the Smart Card should be considered sensitive. false by default.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var isSensitive: Bool { get set }
```

## Discussion

When this property is set to true, any sessions established for the receiver will begin and end by sending a reset command to the Smart Card. This is recommended anytime potentially sensitive information is transferred.

## See Also

### Configuring the Smart Card

var slot: TKSmartCardSlot

The slot in which the Smart Card is inserted.

var isValid: Bool

Whether the Smart Card is valid and accessible from its slot.

var context: Any?

User-specified information. This property is automatically set to `nil` if the Smart Card is removed or another `TKSmartCard` object begins a session.

