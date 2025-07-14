

- UIKit
- UIDevice
-  isBatteryMonitoringEnabled 

Instance Property

# isBatteryMonitoringEnabled

A Boolean value that indicates whether battery monitoring is enabled.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var isBatteryMonitoringEnabled: Bool { get set }
```

## Discussion

Enable battery monitoring if your app needs to be notified of changes to the battery state, or if you want to check the battery charge level.

The default value of this property is false, which:

- Disables the posting of battery-related notifications

- Disables the ability to read battery charge level and battery state

## See Also

### Related Documentation

class let batteryLevelDidChangeNotification: NSNotification.Name

A notification that posts when the battery level changes.

class let batteryStateDidChangeNotification: NSNotification.Name

A notification that posts when battery state changes.

### Getting the device battery state

var batteryLevel: Float

The battery charge level for the device.

var batteryState: UIDevice.BatteryState

The battery state for the device.

enum BatteryState

Constants that describe the battery power state of the device.

