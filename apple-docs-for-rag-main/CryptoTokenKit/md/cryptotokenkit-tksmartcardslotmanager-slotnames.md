

- CryptoTokenKit
- TKSmartCardSlotManager
-  slotNames 

Instance Property

# slotNames

A list of identifiers for all the Smart Card reader slots available to the system.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var slotNames: [String] { get }
```

## Discussion

Use Key-Value Observing on this property to be notified for changes to available Smart Card reader slots. For more information, see Key-Value Observing Programming Guide.

## See Also

### Accessing Smart Card Slots

func getSlot(withName: String, reply: (TKSmartCardSlot?) -> Void)

Asynchronously calls a block with a Smart Card reader slot for a specified name.

func slotNamed(String) -> TKSmartCardSlot?

Returns the Smart Card slot with a given name.

