

- UIKit
- UIAccessibility
- UIAccessibility.GuidedAccessError
-  UIAccessibility.GuidedAccessError.Code 

Enumeration

# UIAccessibility.GuidedAccessError.Code

Error codes for Guided Access.

iOS 12.2+iPadOS 12.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum Code
```

## Topics

### Errors

case permissionDenied

An error that indicates the app isn’t authorized to perform the requested action.

case failed

An error that indicates a failure for an unspecified reason.

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

### Guided Access

static func configureForGuidedAccess(features: UIGuidedAccessAccessibilityFeature, enabled: Bool, completionHandler: (Bool, (any Error)?) -> Void)

Enables or disables the specified accessibility features while using Guided Access.

struct UIGuidedAccessAccessibilityFeature

Constants that describe accessibility features for Guided Access.

