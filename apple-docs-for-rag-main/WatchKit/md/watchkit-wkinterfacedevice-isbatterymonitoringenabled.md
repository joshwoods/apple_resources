

- WatchKit
- WKInterfaceDevice
-  isBatteryMonitoringEnabled 

Instance Property

# isBatteryMonitoringEnabled

A Boolean value that determines whether the app can monitor the device’s battery.

watchOS 4.0+

``` source
var isBatteryMonitoringEnabled: Bool { get set }
```

## Discussion

This property defaults to false. To monitor the device’s battery, set this property to true. This enables both the batteryLevel and batteryState properties.

## See Also

### Reading Information About the Battery

var batteryLevel: Float

The battery’s current percent charge.

var batteryState: WKInterfaceDeviceBatteryState

The device’s battery state.

enum WKInterfaceDeviceBatteryState

The battery’s charging state.

