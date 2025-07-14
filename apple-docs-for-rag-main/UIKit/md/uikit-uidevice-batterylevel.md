

- UIKit
- UIDevice
-  batteryLevel 

Instance Property

# batteryLevel

The battery charge level for the device.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var batteryLevel: Float { get }
```

## Discussion

Battery level ranges from 0.0 (fully discharged) to 1.0 (100% charged). Before accessing this property, ensure that battery monitoring is enabled.

If battery monitoring is not enabled, battery state is UIDevice.BatteryState.unknown and the value of this property is –1.0.

## See Also

### Getting the device battery state

var isBatteryMonitoringEnabled: Bool

A Boolean value that indicates whether battery monitoring is enabled.

var batteryState: UIDevice.BatteryState

The battery state for the device.

enum BatteryState

Constants that describe the battery power state of the device.

