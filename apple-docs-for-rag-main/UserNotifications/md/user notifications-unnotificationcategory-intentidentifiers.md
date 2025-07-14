

- User Notifications
- UNNotificationCategory
-  intentIdentifiers 

Instance Property

# intentIdentifiers

The intents related to notifications of this category.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
var intentIdentifiers: [String] { get }
```

## Discussion

When the system delivers a notification, the presence of an intent identifier lets the system know that the notification is potentially related to the handling of a request made through Siri.

## See Also

### Getting the Information

var identifier: String

The unique string assigned to the category.

var actions: [UNNotificationAction]

The actions to display when the system delivers notifications of this type.

var hiddenPreviewsBodyPlaceholder: String

The placeholder text to display when the system disables notification previews for the app.

var categorySummaryFormat: String

A format string for the summary description used when the system groups the category’s notifications.

