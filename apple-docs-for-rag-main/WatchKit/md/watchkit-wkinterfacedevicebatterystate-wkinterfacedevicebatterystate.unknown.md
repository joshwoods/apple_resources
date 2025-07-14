

- WatchKit
- WKInterfaceDeviceBatteryState
-  WKInterfaceDeviceBatteryState.unknown 

Case

# WKInterfaceDeviceBatteryState.unknown

An unknown battery-charging state.

watchOS 4.0+

``` source
case unknown
```

## Discussion

When the device’s isBatteryMonitoringEnabled property is set to false, its batteryState property is set to WKInterfaceDeviceBatteryState.unknown.

## See Also

### Battery States

case charging

The device is connected to a charger, but its battery charge is under 100%.

case full

The device is connected to a charger, and its battery is charged to 100%.

case unplugged

The device is not connected to a charger and is running on battery power.

