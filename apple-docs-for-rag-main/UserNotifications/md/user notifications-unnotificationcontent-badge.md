

- User Notifications
- UNNotificationContent
-  badge 

Instance Property

# badge

The number that your app’s icon displays.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
@NSCopying
var badge: NSNumber? { get }
```

## Discussion

When the number in this property is `0`, the system doesn’t display a badge. When the number is greater than `0`, the system displays the badge with the specified number. When the value in this property is `nil`, the system leaves the current badge unchanged.

## See Also

### Reading app configuration

var launchImageName: String

The name of the image or storyboard to use when your app launches because of the notification.

var targetContentIdentifier: String?

The value your app uses to determine which scene to display to handle the notification.

