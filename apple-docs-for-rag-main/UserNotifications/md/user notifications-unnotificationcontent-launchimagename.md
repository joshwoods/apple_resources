

- User Notifications
- UNNotificationContent
-  launchImageName 

Instance Property

# launchImageName

The name of the image or storyboard to use when your app launches because of the notification.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 3.0+

``` source
var launchImageName: String { get }
```

## Discussion

If you specify a value for this property, the system displays the specified image or storyboard when the system launches your app. The string in this property must match the name of an image file or storyboard in your app’s bundle.

## See Also

### Reading app configuration

var badge: NSNumber?

The number that your app’s icon displays.

var targetContentIdentifier: String?

The value your app uses to determine which scene to display to handle the notification.

