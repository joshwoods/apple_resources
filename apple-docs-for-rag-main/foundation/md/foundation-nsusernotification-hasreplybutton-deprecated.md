

- Foundation
- NSUserNotification
-  hasReplyButton Deprecated

Instance Property

# hasReplyButton

A Boolean value that specifies whether the notification displays a reply button.

macOS 10.9–11.0Deprecated

``` source
var hasReplyButton: Bool { get set }
```

## Discussion

Set to true if the notification has a reply button. The default value is false. If this property and hasActionButton are both true, the reply button is shown.

## See Also

### Displayed Notification Buttons

var hasActionButton: Bool

A Boolean value that specifies whether the notification displays an action button.

Deprecated

var actionButtonTitle: String

Specifies the title of the action button displayed in the notification.

Deprecated

var otherButtonTitle: String

Specifies a custom title for the close button in an alert-style notification.

Deprecated

