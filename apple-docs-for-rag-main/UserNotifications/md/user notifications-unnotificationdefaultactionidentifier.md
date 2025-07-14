

- User Notifications
-  UNNotificationDefaultActionIdentifier 

Global Variable

# UNNotificationDefaultActionIdentifier

An action that indicates the user opened the app from the notification interface.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
let UNNotificationDefaultActionIdentifier: String
```

## Discussion

The delivery of this action doesn’t require any special configuration of notification categories. Use the userNotificationCenter(_:didReceive:withCompletionHandler:) method of your delegate object to receive this action.

## See Also

### Getting the Response Information

var actionIdentifier: String

The identifier string of the action that the user selected.

var notification: UNNotification

The notification to which the user responded.

var targetScene: UIScene?

The scene where the system reflects the user’s response to a notification.

let UNNotificationDismissActionIdentifier: String

The action that indicates the user explicitly dismissed the notification interface.

