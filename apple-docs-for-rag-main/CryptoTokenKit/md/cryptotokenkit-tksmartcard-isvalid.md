

- CryptoTokenKit
- TKSmartCard
-  isValid 

Instance Property

# isValid

Whether the Smart Card is valid and accessible from its slot.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var isValid: Bool { get }
```

## Discussion

Use Key-Value-Observing to be notified for changes to accessibility, such as when a Smart Card is physically removed from its slot. For more information, see Key-Value Observing Programming Guide.

## See Also

### Configuring the Smart Card

var slot: TKSmartCardSlot

The slot in which the Smart Card is inserted.

var isSensitive: Bool

Whether sessions established for the Smart Card should be considered sensitive. false by default.

var context: Any?

User-specified information. This property is automatically set to `nil` if the Smart Card is removed or another `TKSmartCard` object begins a session.

