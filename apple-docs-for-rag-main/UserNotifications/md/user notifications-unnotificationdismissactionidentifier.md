

- User Notifications
-  UNNotificationDismissActionIdentifier 

Global Variable

# UNNotificationDismissActionIdentifier

The action that indicates the user explicitly dismissed the notification interface.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
let UNNotificationDismissActionIdentifier: String
```

## Discussion

The system delivers this action only if your app configured the notification’s category object with the customDismissAction option. To trigger this action, the user must explicitly dismiss the notification interface. For example, the user must tap the Dismiss button or swipe down on the notification interface in watchOS to trigger this action.

Ignoring a notification or flicking away a notification banner doesn’t trigger this action.

## See Also

### Getting the Response Information

var actionIdentifier: String

The identifier string of the action that the user selected.

var notification: UNNotification

The notification to which the user responded.

var targetScene: UIScene?

The scene where the system reflects the user’s response to a notification.

let UNNotificationDefaultActionIdentifier: String

An action that indicates the user opened the app from the notification interface.

