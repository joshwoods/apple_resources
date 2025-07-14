

- UIKit
- UIDevice
-  proximityStateDidChangeNotification 

Type Property

# proximityStateDidChangeNotification

A notification that posts when the state of the proximity sensor changes.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
nonisolated
class let proximityStateDidChangeNotification: NSNotification.Name
```

## Mentioned in 

Processing queued notifications

## Discussion

You can obtain the proximity state by getting the value of the proximityState property.

## See Also

### Managing notifications

class let batteryLevelDidChangeNotification: NSNotification.Name

A notification that posts when the battery level changes.

class let batteryStateDidChangeNotification: NSNotification.Name

A notification that posts when battery state changes.

class let orientationDidChangeNotification: NSNotification.Name

A notification that posts when the orientation of the device changes.

