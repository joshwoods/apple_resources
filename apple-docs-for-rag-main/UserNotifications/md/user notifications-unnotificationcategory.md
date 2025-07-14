

- User Notifications
-  UNNotificationCategory 

Class

# UNNotificationCategory

A type of notification your app supports and the custom actions that the system displays.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
class UNNotificationCategory
```

## Mentioned in 

Generating a remote notification

Declaring your actionable notification types

## Overview

A UNNotificationCategory object defines a type of notification that your executable can receive. You create category objects to define your app’s *actionable notifications* — notifications that have action buttons the user can select in response to the notification. Each category object you create stores the actions and other behaviors associated with a specific type of notification. Register your category objects using the setNotificationCategories(_:) method of UNUserNotificationCenter. You can register as many category objects as you need.

Note

When someone performs a Double Tap gesture while viewing a notification on Apple Watch Series 9 or Apple Watch Ultra 2, the system invokes the first nondestructive action. A nondestructive action doesn’t include the destructive option, and won’t delete user data or change the app irrevocably.

To apply category objects to your notifications, include the category’s identifier string in the payload of any notifications you create. For local notifications, put this string in the categoryIdentifier property of the UNMutableNotificationContent object that you use to specify the notification’s content. For remote notifications, use this string as the value of the `category` key in the `aps` dictionary of your payload.

Categories can have associated actions, which define custom buttons the system displays for notifications of that category. When the system has unlimited space, the system displays up to 10 actions. When the system has limited space, the system displays at most two actions.

## Topics

### Essentials

convenience init(identifier: String, actions: [UNNotificationAction], intentIdentifiers: [String], options: UNNotificationCategoryOptions)

Creates a category object containing the specified actions and options.

convenience init(identifier: String, actions: [UNNotificationAction], intentIdentifiers: [String], hiddenPreviewsBodyPlaceholder: String, options: UNNotificationCategoryOptions)

Creates a category object containing the specified actions, options, and placeholder text used when previews aren’t shown.

convenience init(identifier: String, actions: [UNNotificationAction], intentIdentifiers: [String], hiddenPreviewsBodyPlaceholder: String?, categorySummaryFormat: String?, options: UNNotificationCategoryOptions)

Creates a category object containing the specified actions, options, placeholder text used when previews aren’t shown, and summary format string.

### Getting the Information

var identifier: String

The unique string assigned to the category.

var actions: [UNNotificationAction]

The actions to display when the system delivers notifications of this type.

var intentIdentifiers: [String]

The intents related to notifications of this category.

var hiddenPreviewsBodyPlaceholder: String

The placeholder text to display when the system disables notification previews for the app.

var categorySummaryFormat: String

A format string for the summary description used when the system groups the category’s notifications.

### Getting the Options

var options: UNNotificationCategoryOptions

Options for how to handle notifications of this type.

struct UNNotificationCategoryOptions

Constants indicating how to handle notifications associated with this category.

## Relationships

### Inherits From

- NSObject

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

class UNNotificationAction

A task your app performs in response to a notification that the system delivers.

class UNTextInputNotificationAction

An action that accepts user-typed text.

