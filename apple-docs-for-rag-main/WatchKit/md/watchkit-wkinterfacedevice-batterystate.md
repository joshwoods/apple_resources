

- WatchKit
- WKInterfaceDevice
-  batteryState 

Instance Property

# batteryState

The device’s battery state.

watchOS 4.0+

``` source
var batteryState: WKInterfaceDeviceBatteryState { get }
```

## Discussion

If battery monitoring is enabled, this property is set to the device’s current battery state. For a list of possible states, see WKInterfaceDeviceBatteryState.

If battery monitoring is disabled, this property is set to WKInterfaceDeviceBatteryState.unknown.

## See Also

### Reading Information About the Battery

var isBatteryMonitoringEnabled: Bool

A Boolean value that determines whether the app can monitor the device’s battery.

var batteryLevel: Float

The battery’s current percent charge.

enum WKInterfaceDeviceBatteryState

The battery’s charging state.

