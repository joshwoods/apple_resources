

- AppKit
- NSAccessibility
- NSAccessibility.NotificationUserInfoKey
-  priority 

Type Property

# priority

A priority level that can help an assistive app determine how to handle the corresponding notification.

macOS 10.9+

``` source
static let priority: NSAccessibility.NotificationUserInfoKey
```

## Discussion

An example of using this key is VoiceOver which decides whether to speak an announcement immediately or after the current speech has finished. For a list of possible values, see NSAccessibilityPriorityLevel.

## See Also

### Constants

static let announcement: NSAccessibility.NotificationUserInfoKey

The announcement as a localized string.

static let uiElements: NSAccessibility.NotificationUserInfoKey

An array of elements for the notification.

enum NSAccessibilityPriorityLevel

A data type for notification priority levels.

