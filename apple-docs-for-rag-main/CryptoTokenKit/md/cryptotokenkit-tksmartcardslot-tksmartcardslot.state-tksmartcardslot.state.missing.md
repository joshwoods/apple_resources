

- CryptoTokenKit
- TKSmartCardSlot
- TKSmartCardSlot.State
-  TKSmartCardSlot.State.missing 

Case

# TKSmartCardSlot.State.missing

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
case missing
```

## Discussion

The Smart Card reader slot is no longer known to the system.

Important

This is the terminal state of a `TKSmartCardSlotThis` instance; once it has reached this state, the Smart Card reader slot cannot be reinitialized.

## See Also

### Constants

case empty

case probing

case muteCard

case validCard

