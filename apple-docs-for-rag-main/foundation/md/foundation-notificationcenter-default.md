

- Foundation
- NotificationCenter
-  default 

Type Property

# default

The app’s default notification center.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class var `default`: NotificationCenter { get }
```

## Discussion

All system notifications sent to an app are posted to the default notification center. You can also post your own notifications there.

If your app uses notifications extensively, you may want to create and post to your own notification centers rather than posting only to the default notification center. When a notification is posted to a notification center, the notification center scans through the list of registered observers, which may slow down your app. By organizing notifications functionally around one or more notification centers, less work is done each time a notification is posted, which can improve performance throughout your app.

## See Also

### Related Documentation

Notification Programming Topics

