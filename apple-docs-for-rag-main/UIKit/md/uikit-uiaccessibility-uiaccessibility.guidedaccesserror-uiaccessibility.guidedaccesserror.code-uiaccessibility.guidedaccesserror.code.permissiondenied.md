

- UIKit
- UIAccessibility
- UIAccessibility.GuidedAccessError
- UIAccessibility.GuidedAccessError.Code
-  UIAccessibility.GuidedAccessError.Code.permissionDenied 

Case

# UIAccessibility.GuidedAccessError.Code.permissionDenied

An error that indicates the app isn’t authorized to perform the requested action.

iOS 12.2+iPadOS 12.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
case permissionDenied
```

## Discussion

For example, this error might indicate that your app is requesting a configuration change but isn’t locked into Single App Mode through a configuration profile.

## See Also

### Errors

case failed

An error that indicates a failure for an unspecified reason.

