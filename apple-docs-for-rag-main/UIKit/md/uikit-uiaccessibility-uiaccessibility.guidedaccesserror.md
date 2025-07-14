

- UIKit
- UIAccessibility
-  UIAccessibility.GuidedAccessError 

Structure

# UIAccessibility.GuidedAccessError

A Guided Access error.

iOS 12.2+iPadOS 12.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
struct GuidedAccessError
```

## Topics

### Accessing error codes

static var permissionDenied: UIAccessibility.GuidedAccessError.Code

An error that indicates the app isn’t authorized to perform the requested action.

static var failed: UIAccessibility.GuidedAccessError.Code

An error that indicates a failure for an unspecified reason.

enum Code

Error codes for Guided Access.

### Getting error information

static var errorDomain: String

The Guided Access error domain.

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

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

static let guidedAccessErrorDomain: String

A string that identifies the Guided Access error domain.

