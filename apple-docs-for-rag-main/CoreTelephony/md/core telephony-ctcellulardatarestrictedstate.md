

- Core Telephony
-  CTCellularDataRestrictedState 

Enumeration

# CTCellularDataRestrictedState

The possible states of the cellular data policy.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.10+

``` source
enum CTCellularDataRestrictedState
```

## Topics

### Constants

case notRestricted

A state that allows access to cellular data.

case restricted

A state that denies access to cellular data.

case restrictedStateUnknown

A state whose access to cellular data is unknown.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Determining the Cellular Data Restricted State

var restrictedState: CTCellularDataRestrictedState

The current state of cellular data restrictions.

