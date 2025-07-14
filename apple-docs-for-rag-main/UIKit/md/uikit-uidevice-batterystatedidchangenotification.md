

- UIKit
- UIDevice
-  batteryStateDidChangeNotification 

Type Property

# batteryStateDidChangeNotification

A notification that posts when battery state changes.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
nonisolated
class let batteryStateDidChangeNotification: NSNotification.Name
```

## Mentioned in 

Processing queued notifications

## Discussion

For this notification to be sent, you must set the isBatteryMonitoringEnabled property to true.

You can obtain the battery state by getting the value of the batteryState property.

## See Also

### Managing notifications

class let batteryLevelDidChangeNotification: NSNotification.Name

A notification that posts when the battery level changes.

class let orientationDidChangeNotification: NSNotification.Name

A notification that posts when the orientation of the device changes.

class let proximityStateDidChangeNotification: NSNotification.Name

A notification that posts when the state of the proximity sensor changes.

