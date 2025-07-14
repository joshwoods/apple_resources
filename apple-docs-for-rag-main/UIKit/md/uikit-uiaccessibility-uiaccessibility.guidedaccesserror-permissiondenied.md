

- UIKit
- UIAccessibility
- UIAccessibility.GuidedAccessError
-  permissionDenied 

Type Property

# permissionDenied

An error that indicates the app isn’t authorized to perform the requested action.

iOS 12.2+iPadOS 12.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
static var permissionDenied: UIAccessibility.GuidedAccessError.Code { get }
```

## Discussion

For example, this error might indicate that your app is requesting a configuration change but isn’t locked into Single App Mode through a configuration profile.

## See Also

### Accessing error codes

static var failed: UIAccessibility.GuidedAccessError.Code

An error that indicates a failure for an unspecified reason.

enum Code

Error codes for Guided Access.

