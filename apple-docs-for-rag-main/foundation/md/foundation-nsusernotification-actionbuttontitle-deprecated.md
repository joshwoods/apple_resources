

- Foundation
- NSUserNotification
-  actionButtonTitle Deprecated

Instance Property

# actionButtonTitle

Specifies the title of the action button displayed in the notification.

macOS 10.8–11.0Deprecated

``` source
var actionButtonTitle: String { get set }
```

Deprecated

All NSUserNotifications API should be replaced with UserNotifications.frameworks API

## Discussion

This value should be localized as it is presented to the user. The string is truncated to a length appropriate for display and the property is modified to reflect the truncation.

## See Also

### Displayed Notification Buttons

var hasActionButton: Bool

A Boolean value that specifies whether the notification displays an action button.

Deprecated

var otherButtonTitle: String

Specifies a custom title for the close button in an alert-style notification.

Deprecated

var hasReplyButton: Bool

A Boolean value that specifies whether the notification displays a reply button.

Deprecated

