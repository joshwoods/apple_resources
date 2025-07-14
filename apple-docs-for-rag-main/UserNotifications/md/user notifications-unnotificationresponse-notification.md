

- User Notifications
- UNNotificationResponse
-  notification 

Instance Property

# notification

The notification to which the user responded.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
@NSCopying
var notification: UNNotification { get }
```

## See Also

### Getting the Response Information

var actionIdentifier: String

The identifier string of the action that the user selected.

var targetScene: UIScene?

The scene where the system reflects the user’s response to a notification.

let UNNotificationDefaultActionIdentifier: String

An action that indicates the user opened the app from the notification interface.

let UNNotificationDismissActionIdentifier: String

The action that indicates the user explicitly dismissed the notification interface.

