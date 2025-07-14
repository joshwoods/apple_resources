

- UIKit
- UIAccessibility
-  configureForGuidedAccess(features:enabled:completionHandler:) 

Type Method

# configureForGuidedAccess(features:enabled:completionHandler:)

Enables or disables the specified accessibility features while using Guided Access.

iOS 12.2+iPadOS 12.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
static func configureForGuidedAccess(
    features: UIGuidedAccessAccessibilityFeature,
    enabled: Bool,
    completionHandler completion: @escaping (Bool, (any Error)?) -> Void
)
```

## See Also

### Guided Access

struct UIGuidedAccessAccessibilityFeature

Constants that describe accessibility features for Guided Access.

enum Code

Error codes for Guided Access.

