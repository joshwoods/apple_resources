

- UIKit
- UIDevice
-  batteryState 

Instance Property

# batteryState

The battery state for the device.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var batteryState: UIDevice.BatteryState { get }
```

## Discussion

The value for batteryState is one of the constants in UIDevice.BatteryState.

If battery monitoring is not enabled, the value of this property is UIDevice.BatteryState.unknown.

## See Also

### Getting the device battery state

var batteryLevel: Float

The battery charge level for the device.

var isBatteryMonitoringEnabled: Bool

A Boolean value that indicates whether battery monitoring is enabled.

enum BatteryState

Constants that describe the battery power state of the device.

