

- AppKit
- NSAccessibility
- NSAccessibility.NotificationUserInfoKey
-  uiElements 

Type Property

# uiElements

An array of elements for the notification.

macOS 10.9+

``` source
static let uiElements: NSAccessibility.NotificationUserInfoKey
```

## Discussion

The value is an array of accessibility elements for the notification. For example, in the layoutChanged notification, use this key to include an array of elements that you add or change.

## See Also

### Constants

static let announcement: NSAccessibility.NotificationUserInfoKey

The announcement as a localized string.

static let priority: NSAccessibility.NotificationUserInfoKey

A priority level that can help an assistive app determine how to handle the corresponding notification.

enum NSAccessibilityPriorityLevel

A data type for notification priority levels.

