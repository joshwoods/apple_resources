

- AppKit
- NSAccessibility
-  post(element:notification:userInfo:) 

Type Method

# post(element:notification:userInfo:)

Sends a notification and an optional user info dictionary to any observing assistive apps.

macOS 10.7+

``` source
static func post(
    element: Any,
    notification: NSAccessibility.Notification,
    userInfo: [NSAccessibility.NotificationUserInfoKey : Any]?
)
```

## Discussion

Sends `notification` and `userInfo` to any assistive apps that register to receive the notification from the UI object `element` in your app. The system restricts the `userInfo` dictionary values to the same values as it restricts the accessibility attributes. The `userInfo` dictionary can also be `nil` (most accessibility notifications don’t require it).

## See Also

### Posting Notifications

static func post(element: Any, notification: NSAccessibility.Notification)

Sends a notification to any observing assistive apps.

