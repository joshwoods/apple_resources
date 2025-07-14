

- Foundation
- NSUserNotification
-  otherButtonTitle Deprecated

Instance Property

# otherButtonTitle

Specifies a custom title for the close button in an alert-style notification.

macOS 10.8–11.0Deprecated

``` source
var otherButtonTitle: String { get set }
```

Deprecated

All NSUserNotifications API should be replaced with UserNotifications.frameworks API

## Discussion

This value should be localized as it is presented to the user. The string is truncated to a length appropriate for display and the property is modified to reflect the truncation.

An empty string will cause the default localized text to be used. A `nil` value is invalid.

## See Also

### Displayed Notification Buttons

var hasActionButton: Bool

A Boolean value that specifies whether the notification displays an action button.

Deprecated

var actionButtonTitle: String

Specifies the title of the action button displayed in the notification.

Deprecated

var hasReplyButton: Bool

A Boolean value that specifies whether the notification displays a reply button.

Deprecated

