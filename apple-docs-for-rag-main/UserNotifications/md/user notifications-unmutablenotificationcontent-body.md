

- User Notifications
- UNMutableNotificationContent
-  body 

Instance Property

# body

The localized text that provides the notification’s main content.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
var body: String { get set }
```

## Discussion

Use this property to specify the body of the notification alert. If your app isn’t authorized to display alert-based notifications, the system ignores this property.

The body text should contain the final text that you want to display, and shouldn’t contain any placeholder characters. To include a percent symbol (`%`) in the message body, use two percent symbols (`%%`). The system strips all other printf style escape characters from your string prior to display.

## See Also

### Providing the primary content

var title: String

The localized text that provides the notification’s primary description.

var subtitle: String

The localized text that provides the notification’s secondary description.

