

- User Notifications
- UNNotificationResponse
-  actionIdentifier 

Instance Property

# actionIdentifier

The identifier string of the action that the user selected.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
var actionIdentifier: String { get }
```

## Mentioned in 

Declaring your actionable notification types

Handling notifications and notification-related actions

## Discussion

This parameter may contain one the identifier of one of your UNNotificationAction objects or it may contain a system-defined identifier. The system defined identifiers are UNNotificationDefaultActionIdentifier and UNNotificationDismissActionIdentifier, which indicate that the user opened the app or dismissed the notification without any further actions.

For more information about defining custom actions, see Declaring your actionable notification types.

## See Also

### Getting the Response Information

var notification: UNNotification

The notification to which the user responded.

var targetScene: UIScene?

The scene where the system reflects the user’s response to a notification.

let UNNotificationDefaultActionIdentifier: String

An action that indicates the user opened the app from the notification interface.

let UNNotificationDismissActionIdentifier: String

The action that indicates the user explicitly dismissed the notification interface.

