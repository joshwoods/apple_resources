

- CryptoTokenKit
- TKSmartCardSlotManager
-  slotNamed(\_:) 

Instance Method

# slotNamed(\_:)

Returns the Smart Card slot with a given name.

iOSiPadOSMac Catalyst 13.1+macOS 10.13+tvOSvisionOSwatchOS

``` source
func slotNamed(_ name: String) -> TKSmartCardSlot?
```

## Return Value

The slot with the specified name, or `nil` if no slot with that name exists.

## See Also

### Accessing Smart Card Slots

var slotNames: [String]

A list of identifiers for all the Smart Card reader slots available to the system.

func getSlot(withName: String, reply: (TKSmartCardSlot?) -> Void)

Asynchronously calls a block with a Smart Card reader slot for a specified name.

