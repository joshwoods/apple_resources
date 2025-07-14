

- User Notifications
- UNMutableNotificationContent
-  sound 

Instance Property

# sound

The sound that plays when the system delivers the notification.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
@NSCopying
var sound: UNNotificationSound? { get set }
```

## Discussion

Use this property to specify the sound that you want played when the notification arrives. If your app isn’t authorized to play sounds for notifications, the system ignores this property.

For information on how to specify sounds for your notifications, see UNNotificationSound.

## See Also

### Integrating with the system

var interruptionLevel: UNNotificationInterruptionLevel

The notification’s importance and required delivery timing.

enum UNNotificationInterruptionLevel

Constants that indicate the importance and delivery timing of a notification.

var relevanceScore: Double

The score the system uses to determine if the notification is the summary’s featured notification.

var filterCriteria: String?

The criteria the system evaluates to determine if it displays the notification in the current Focus.

