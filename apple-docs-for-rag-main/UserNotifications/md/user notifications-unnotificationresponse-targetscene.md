

- User Notifications
- UNNotificationResponse
-  targetScene 

Instance Property

# targetScene

The scene where the system reflects the user’s response to a notification.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var targetScene: UIScene? { get }
```

## See Also

### Getting the Response Information

var actionIdentifier: String

The identifier string of the action that the user selected.

var notification: UNNotification

The notification to which the user responded.

let UNNotificationDefaultActionIdentifier: String

An action that indicates the user opened the app from the notification interface.

let UNNotificationDismissActionIdentifier: String

The action that indicates the user explicitly dismissed the notification interface.

