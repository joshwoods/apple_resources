

- UIKit
- UIAccessibility
-  guidedAccessErrorDomain 

Type Property

# guidedAccessErrorDomain

A string that identifies the Guided Access error domain.

iOS 12.2+iPadOS 12.2+Mac Catalyst 13.1+tvOS 12.2+visionOS 1.0+

``` source
nonisolated
static let guidedAccessErrorDomain: String
```

## See Also

### Guided Access

static var isGuidedAccessEnabled: Bool

A Boolean value that indicates whether the Guided Access setting is in an enabled state.

static let guidedAccessStatusDidChangeNotification: NSNotification.Name

A notification that indicates when a Guided Access session starts or ends.

static func requestGuidedAccessSession(enabled: Bool, completionHandler: (Bool) -> Void)

Transitions the app to or from Single App mode asynchronously.

static func configureForGuidedAccess(features: UIGuidedAccessAccessibilityFeature, enabled: Bool, completionHandler: (Bool, (any Error)?) -> Void)

Enables or disables the specified accessibility features while using Guided Access.

static func guidedAccessRestrictionState(forIdentifier: String) -> UIAccessibility.GuidedAccessRestrictionState

Returns the restriction state for the specified guided access restriction.

enum GuidedAccessRestrictionState

Constants that describe the state of a restriction, either allow or deny.

struct GuidedAccessError

A Guided Access error.

