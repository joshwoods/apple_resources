

- Core Foundation
- CFNotificationName
-  cfTimeZoneSystemTimeZoneDidChange 

Type Property

# cfTimeZoneSystemTimeZoneDidChange

Name of the notification posted when the system time zone changes.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let cfTimeZoneSystemTimeZoneDidChange: CFNotificationName!
```

## Discussion

The object of the notification is the previous system time zone object. This notification carries no user info.

Keep in mind that there is no order in how notifications are delivered to observers; frameworks or other parts of your code may also be observing this notification to take their own actions, and these may not have occurred by the time you receive the notification.

