

- User Notifications
-  UNTextInputNotificationAction 

Class

# UNTextInputNotificationAction

An action that accepts user-typed text.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
class UNTextInputNotificationAction
```

## Mentioned in 

Declaring your actionable notification types

## Overview

Use UNTextInputNotificationAction objects to define an action that allows the user to provide a custom text-based response. When the user selects an action of this type, the system displays controls for the user to enter or dictate the text content. That text is then included in the response object that’s delivered to your app.

For information on how to define actions and categories, see Declaring your actionable notification types.

## Topics

### Essentials

convenience init(identifier: String, title: String, options: UNNotificationActionOptions, textInputButtonTitle: String, textInputPlaceholder: String)

Creates an action object that accepts text input from the user.

convenience init(identifier: String, title: String, options: UNNotificationActionOptions, icon: UNNotificationActionIcon?, textInputButtonTitle: String, textInputPlaceholder: String)

Creates an action object with an icon that accepts text input from the user.

### Getting Information

var textInputButtonTitle: String

The localized title of the text input button that the system displays to the user.

var textInputPlaceholder: String

The placeholder text that the system localizes and displays in the text input field.

## Relationships

### Inherits From

- UNNotificationAction

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

class UNNotificationAction

A task your app performs in response to a notification that the system delivers.

