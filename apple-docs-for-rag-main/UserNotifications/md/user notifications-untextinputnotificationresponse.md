

- User Notifications
-  UNTextInputNotificationResponse 

Class

# UNTextInputNotificationResponse

The user’s response to an actionable notification, including any custom text that the user typed or dictated.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
class UNTextInputNotificationResponse
```

## Overview

The system delivers a UNTextInputNotificationResponse object to your app so that you can process user-provided text content. When defining your categories, you can specify an UNTextInputNotificationAction object instead of an UNNotificationAction object for your action. If you do, the system creates an UNTextInputNotificationResponse object when the user selects the accompanying action, and it fills the userText property with any user-entered text.

You don’t create UNTextInputNotificationResponse objects yourself. Instead, the shared user notification center object creates them and delivers them to the userNotificationCenter(_:didReceive:withCompletionHandler:) method of its delegate object. Use that method to extract any needed information from the response object and take appropriate action.

For more information about responding to actions, see Handling notifications and notification-related actions.

## Topics

### Getting the Text Response

var userText: String

The text response provided by the user.

## Relationships

### Inherits From

- UNNotificationResponse

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

class UNNotificationResponse

The user’s response to an actionable notification.

