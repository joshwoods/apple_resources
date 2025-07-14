

- User Notifications
- UNNotificationContent
-  filterCriteria 

Instance Property

# filterCriteria

The criteria the system evaluates to determine if it displays the notification in the current Focus.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+watchOS 9.0+

``` source
var filterCriteria: String? { get }
```

## Discussion

For more information, see SetFocusFilterIntent.

## See Also

### Reading system configuration

var sound: UNNotificationSound?

The sound that plays when the system delivers the notification.

var interruptionLevel: UNNotificationInterruptionLevel

The notification’s importance and required delivery timing.

enum UNNotificationInterruptionLevel

Constants that indicate the importance and delivery timing of a notification.

var relevanceScore: Double

The score the system uses to determine if the notification is the summary’s featured notification.

