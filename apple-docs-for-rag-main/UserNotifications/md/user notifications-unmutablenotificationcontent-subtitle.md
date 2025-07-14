

- User Notifications
- UNMutableNotificationContent
-  subtitle 

Instance Property

# subtitle

The localized text that provides the notification’s secondary description.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
var subtitle: String { get set }
```

## Discussion

Use this property to specify additional context about the purpose of the notification. Subtitles offer additional context in cases where the title alone isn’t clear. Subtitles aren’t displayed in all cases. If your app isn’t authorized to display alert-based notifications, the system ignores this property.

## See Also

### Providing the primary content

var title: String

The localized text that provides the notification’s primary description.

var body: String

The localized text that provides the notification’s main content.

