

- CryptoTokenKit
- TKSmartCardSlot
-  TKSmartCardSlot.State 

Enumeration

# TKSmartCardSlot.State

All smart card slot states.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
enum State
```

## Topics

### Constants

case missing

case empty

case probing

case muteCard

case validCard

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the Slot State

var state: TKSmartCardSlot.State

The current state of the Smart Card reader slot.

