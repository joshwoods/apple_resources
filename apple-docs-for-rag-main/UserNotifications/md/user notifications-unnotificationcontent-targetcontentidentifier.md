

- User Notifications
- UNNotificationContent
-  targetContentIdentifier 

Instance Property

# targetContentIdentifier

The value your app uses to determine which scene to display to handle the notification.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.14+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var targetContentIdentifier: String? { get }
```

## Mentioned in 

Generating a remote notification

## Discussion

Use this value to determine the content to show in your app when the user taps the notification.

## See Also

### Reading app configuration

var launchImageName: String

The name of the image or storyboard to use when your app launches because of the notification.

var badge: NSNumber?

The number that your app’s icon displays.

