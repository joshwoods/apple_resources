

- User Notifications
- UNNotificationContent
-  interruptionLevel 

Instance Property

# interruptionLevel

The notification’s importance and required delivery timing.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var interruptionLevel: UNNotificationInterruptionLevel { get }
```

## See Also

### Reading system configuration

var sound: UNNotificationSound?

The sound that plays when the system delivers the notification.

enum UNNotificationInterruptionLevel

Constants that indicate the importance and delivery timing of a notification.

var relevanceScore: Double

The score the system uses to determine if the notification is the summary’s featured notification.

var filterCriteria: String?

The criteria the system evaluates to determine if it displays the notification in the current Focus.

