

- UIKit
- UIDevice
-  orientationDidChangeNotification 

Type Property

# orientationDidChangeNotification

A notification that posts when the orientation of the device changes.

iOSiPadOSMac Catalyst

``` source
nonisolated
class let orientationDidChangeNotification: NSNotification.Name
```

## Mentioned in 

Processing queued notifications

## Discussion

You can obtain the new orientation by getting the value of the orientation property.

## See Also

### Managing notifications

class let batteryLevelDidChangeNotification: NSNotification.Name

A notification that posts when the battery level changes.

class let batteryStateDidChangeNotification: NSNotification.Name

A notification that posts when battery state changes.

class let proximityStateDidChangeNotification: NSNotification.Name

A notification that posts when the state of the proximity sensor changes.

