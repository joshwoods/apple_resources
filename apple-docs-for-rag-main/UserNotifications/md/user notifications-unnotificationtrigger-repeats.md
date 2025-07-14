

- User Notifications
- UNNotificationTrigger
-  repeats 

Instance Property

# repeats

A Boolean value indicating whether the system reschedules the notification after it’s delivered.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var repeats: Bool { get }
```

## Discussion

When this property is false, the system delivers the notification only once. When this property is true, the system reschedules the notification request automatically, resulting in the system delivering the notification each time the trigger condition is met. To unschedule the notification request, use the methods of the UNUserNotificationCenter to remove the notification request.

