

- User Notifications
- UNNotificationContent
-  relevanceScore 

Instance Property

# relevanceScore

The score the system uses to determine if the notification is the summary’s featured notification.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var relevanceScore: Double { get }
```

## Mentioned in 

Generating a remote notification

## Discussion

The system uses the `relevanceScore`, a value between `0` and `1`, to sort the notifications from your app. The highest score gets featured in the notification summary.

## See Also

### Reading system configuration

var sound: UNNotificationSound?

The sound that plays when the system delivers the notification.

var interruptionLevel: UNNotificationInterruptionLevel

The notification’s importance and required delivery timing.

enum UNNotificationInterruptionLevel

Constants that indicate the importance and delivery timing of a notification.

var filterCriteria: String?

The criteria the system evaluates to determine if it displays the notification in the current Focus.

