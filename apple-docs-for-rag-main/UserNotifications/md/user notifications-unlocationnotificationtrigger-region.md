

- User Notifications
- UNLocationNotificationTrigger
-  region 

Instance Property

# region

The region used to determine when the system sends the notification.

iOS 10.0+iPadOS 10.0+watchOS 3.0+

``` source
@NSCopying
var region: CLRegion { get }
```

## Discussion

Use the notifyOnEntry and notifyOnExit properties of this region to specify whether the system sends notifications when the user enters or exits the specified geographic area.

