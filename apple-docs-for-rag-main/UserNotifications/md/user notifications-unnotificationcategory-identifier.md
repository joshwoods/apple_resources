

- User Notifications
- UNNotificationCategory
-  identifier 

Instance Property

# identifier

The unique string assigned to the category.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
var identifier: String { get }
```

## Mentioned in 

Generating a remote notification

Declaring your actionable notification types

## Discussion

Use this string to differentiate the different types of notifications that your app can send. To assign a category to a local notification, assign this string to the categoryIdentifier property of the content object. To assign a category to a remote notification, use the string as the value of the `category` key in the notification payload `aps` dictionary.

## See Also

### Getting the Information

var actions: [UNNotificationAction]

The actions to display when the system delivers notifications of this type.

var intentIdentifiers: [String]

The intents related to notifications of this category.

var hiddenPreviewsBodyPlaceholder: String

The placeholder text to display when the system disables notification previews for the app.

var categorySummaryFormat: String

A format string for the summary description used when the system groups the category’s notifications.

