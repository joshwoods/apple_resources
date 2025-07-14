

- Foundation
- NSUserNotification
-  hasActionButton Deprecated

Instance Property

# hasActionButton

A Boolean value that specifies whether the notification displays an action button.

macOS 10.8–11.0Deprecated

``` source
var hasActionButton: Bool { get set }
```

Deprecated

All NSUserNotifications API should be replaced with UserNotifications.frameworks API

## Discussion

Set to false if the notification has no action button. This is the case for notifications that are purely for information and have no user action. The default value is true.

## See Also

### Displayed Notification Buttons

var actionButtonTitle: String

Specifies the title of the action button displayed in the notification.

Deprecated

var otherButtonTitle: String

Specifies a custom title for the close button in an alert-style notification.

Deprecated

var hasReplyButton: Bool

A Boolean value that specifies whether the notification displays a reply button.

Deprecated

