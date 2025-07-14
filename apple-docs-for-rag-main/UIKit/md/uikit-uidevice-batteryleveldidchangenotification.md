

- UIKit
- UIDevice
-  batteryLevelDidChangeNotification 

Type Property

# batteryLevelDidChangeNotification

A notification that posts when the battery level changes.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
nonisolated
class let batteryLevelDidChangeNotification: NSNotification.Name
```

## Mentioned in 

Processing queued notifications

## Discussion

For this notification to be sent, you must set the isBatteryMonitoringEnabled property to true.

Notifications for battery level change are sent no more frequently than once per minute. Don’t attempt to calculate battery drainage rate or battery time remaining; drainage rate can change frequently depending on built-in applications as well as your application.

You can obtain the battery level by getting the value of the batteryLevel property.

## See Also

### Managing notifications

class let batteryStateDidChangeNotification: NSNotification.Name

A notification that posts when battery state changes.

class let orientationDidChangeNotification: NSNotification.Name

A notification that posts when the orientation of the device changes.

class let proximityStateDidChangeNotification: NSNotification.Name

A notification that posts when the state of the proximity sensor changes.

