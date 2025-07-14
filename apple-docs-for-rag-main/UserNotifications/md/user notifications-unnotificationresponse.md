

- User Notifications
-  UNNotificationResponse 

Class

# UNNotificationResponse

The user’s response to an actionable notification.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
class UNNotificationResponse
```

## Overview

When the user interacts with a delivered notification, the system delivers a UNNotificationResponse object to your app so that you can process the response. Users can interact with delivered notifications in many ways. If the notification’s category had associated action buttons, they can select one of those buttons. Users can also dismiss the notification without selecting one of your actions and they can open your app. A response object tells you which option the user selected.

You don’t create UNNotificationResponse objects yourself. Instead, the shared user notification center object creates them and delivers them to the userNotificationCenter(_:didReceive:withCompletionHandler:) method of its delegate object. Use that method to extract any needed information from the response object and take appropriate action.

For more information about responding to actions, see Handling notifications and notification-related actions.

## Topics

### Getting the Response Information

var actionIdentifier: String

The identifier string of the action that the user selected.

var notification: UNNotification

The notification to which the user responded.

var targetScene: UIScene?

The scene where the system reflects the user’s response to a notification.

let UNNotificationDefaultActionIdentifier: String

An action that indicates the user opened the app from the notification interface.

let UNNotificationDismissActionIdentifier: String

The action that indicates the user explicitly dismissed the notification interface.

## Relationships

### Inherits From

- NSObject

### Inherited By

- UNTextInputNotificationResponse

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Notification responses

Handling notifications and notification-related actions

Respond to user interactions with the system’s notification interfaces, including handling your app’s custom actions.

class UNTextInputNotificationResponse

The user’s response to an actionable notification, including any custom text that the user typed or dictated.

