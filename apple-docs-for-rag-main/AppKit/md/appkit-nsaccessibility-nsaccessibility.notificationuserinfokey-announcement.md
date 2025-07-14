

- AppKit
- NSAccessibility
- NSAccessibility.NotificationUserInfoKey
-  announcement 

Type Property

# announcement

The announcement as a localized string.

macOS 10.7+

``` source
static let announcement: NSAccessibility.NotificationUserInfoKey
```

## Discussion

This key is required for NSAccessibilityProtocol and should be used in conjunction with priority to help assistive apps determine the importance of the announcement.

## See Also

### Constants

static let uiElements: NSAccessibility.NotificationUserInfoKey

An array of elements for the notification.

static let priority: NSAccessibility.NotificationUserInfoKey

A priority level that can help an assistive app determine how to handle the corresponding notification.

enum NSAccessibilityPriorityLevel

A data type for notification priority levels.

