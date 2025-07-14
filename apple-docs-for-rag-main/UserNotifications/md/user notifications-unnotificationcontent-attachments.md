

- User Notifications
- UNNotificationContent
-  attachments 

Instance Property

# attachments

The visual and audio attachments to display alongside the notification’s main content.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
var attachments: [UNNotificationAttachment] { get }
```

## Discussion

Use this property to retrieve the images, movies, and audio files associated with your notification’s content. A notification content app extension might use these values to add the associated content to its view controller.

## See Also

### Accessing supplementary content

var userInfo: [AnyHashable : Any]

The custom data to associate with the notification.

