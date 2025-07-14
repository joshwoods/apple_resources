

- AppKit
- NSAccessibility
-  post(element:notification:) 

Type Method

# post(element:notification:)

Sends a notification to any observing assistive apps.

macOS

``` source
static func post(
    element: Any,
    notification: NSAccessibility.Notification
)
```

## Discussion

Sends `notification` to any assistive applications that register to receive the notification from the user interface object `element` in your app. Accessibility notifications require special handling, so they can’t post using NotificationCenter.

## See Also

### Posting Notifications

static func post(element: Any, notification: NSAccessibility.Notification, userInfo: [NSAccessibility.NotificationUserInfoKey : Any]?)

Sends a notification and an optional user info dictionary to any observing assistive apps.

