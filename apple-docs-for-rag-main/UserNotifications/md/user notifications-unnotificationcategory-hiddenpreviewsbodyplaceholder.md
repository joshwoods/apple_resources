

- User Notifications
- UNNotificationCategory
-  hiddenPreviewsBodyPlaceholder 

Instance Property

# hiddenPreviewsBodyPlaceholder

The placeholder text to display when the system disables notification previews for the app.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+

``` source
var hiddenPreviewsBodyPlaceholder: String { get }
```

## Discussion

The string in this property may contain the special characters `%u` as a placeholder for the number of messages with the same thread identifier. If your app declares this string in a `.stringsdict` property list, the system formats the preview message using the information in that file. For more information about specifying a `.stringsdict` property file, see Internationalization and Localization Guide.

## See Also

### Getting the Information

var identifier: String

The unique string assigned to the category.

var actions: [UNNotificationAction]

The actions to display when the system delivers notifications of this type.

var intentIdentifiers: [String]

The intents related to notifications of this category.

var categorySummaryFormat: String

A format string for the summary description used when the system groups the category’s notifications.

