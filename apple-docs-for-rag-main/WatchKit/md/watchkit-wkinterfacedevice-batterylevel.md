

- WatchKit
- WKInterfaceDevice
-  batteryLevel 

Instance Property

# batteryLevel

The battery’s current percent charge.

watchOS 4.0+

``` source
var batteryLevel: Float { get }
```

## Discussion

If battery monitoring is enabled, this property is set to a value between `0.0` (0% charge) and `1.0` (100% charge). When the batteryState property is set to WKInterfaceDeviceBatteryState.unknown (for example, when battery monitoring is disabled), the value is `-1.0`.

## See Also

### Reading Information About the Battery

var isBatteryMonitoringEnabled: Bool

A Boolean value that determines whether the app can monitor the device’s battery.

var batteryState: WKInterfaceDeviceBatteryState

The device’s battery state.

enum WKInterfaceDeviceBatteryState

The battery’s charging state.

