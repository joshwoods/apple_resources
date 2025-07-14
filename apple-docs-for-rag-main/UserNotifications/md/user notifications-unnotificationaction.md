

- User Notifications
-  UNNotificationAction 

Class

# UNNotificationAction

A task your app performs in response to a notification that the system delivers.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
class UNNotificationAction
```

## Mentioned in 

Declaring your actionable notification types

## Overview

Use UNNotificationAction objects to define the actions that your app can perform in response to a delivered notification. You define the actions that your app supports. For example, a meeting app might define actions for accepting or rejecting a meeting invitation. The action object itself contains the title to display in an action button and the button’s appearance. After creating action objects, add them to a UNNotificationCategory object and register your categories with the system.

Note

When someone performs a Double Tap gesture while viewing a notification on Apple Watch Series 9 or Apple Watch Ultra 2, the system invokes the first nondestructive action. A nondestructive action doesn’t include the destructive option, and won’t delete user data or change the app irrevocably.

For information on how to define actions and categories, see Declaring your actionable notification types.

### Responding to the Selection of Actions

When the user selects one of your actions in response to a notification, the system notifies the delegate of the shared UNUserNotificationCenter object. Specifically, the system calls the userNotificationCenter(_:didReceive:withCompletionHandler:) method of your delegate object. The response object passed to your delegate includes the identifier string of the action the user selects, which you can use to perform the corresponding task.

For information on how to handle actions, see Handling notifications and notification-related actions.

## Topics

### Essentials

convenience init(identifier: String, title: String, options: UNNotificationActionOptions)

Creates an action object by using the specified title and options.

convenience init(identifier: String, title: String, options: UNNotificationActionOptions, icon: UNNotificationActionIcon?)

Creates an action object by using the specified title, options, and icon.

### Getting Information

var identifier: String

The unique string that your app uses to identify the action.

var title: String

The localized string to use as the title of the action.

var icon: UNNotificationActionIcon?

The icon associated with the action.

### Getting Options

var options: UNNotificationActionOptions

The behaviors associated with the action.

struct UNNotificationActionOptions

The behaviors you can apply to an action.

## Relationships

### Inherits From

- NSObject

### Inherited By

- UNTextInputNotificationAction

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

### Notification categories and user actions

Declaring your actionable notification types

Differentiate your notifications and add action buttons to the notification interface.

class UNNotificationCategory

A type of notification your app supports and the custom actions that the system displays.

class UNTextInputNotificationAction

An action that accepts user-typed text.

