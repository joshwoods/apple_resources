

- UIKit
- UIAccessibility
-  UIAccessibility.GuidedAccessRestrictionState 

Enumeration

# UIAccessibility.GuidedAccessRestrictionState

Constants that describe the state of a restriction, either allow or deny.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum GuidedAccessRestrictionState
```

## Topics

### Constants

case allow

The app should allow the user to perform the action controlled by the restriction.

case deny

The app should deny the user from performing the action controlled by the restriction.

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

### Implementing restrictions

func guidedAccessRestriction(withIdentifier: String, didChange: UIAccessibility.GuidedAccessRestrictionState)

Tells the delegate that the restriction associated with the identifier has changed state.

**Required**

