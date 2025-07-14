

- WatchKit
-  WKInterfaceDeviceBatteryState 

Enumeration

# WKInterfaceDeviceBatteryState

The battery’s charging state.

watchOS 4.0+

``` source
enum WKInterfaceDeviceBatteryState
```

## Topics

### Battery States

case charging

The device is connected to a charger, but its battery charge is under 100%.

case full

The device is connected to a charger, and its battery is charged to 100%.

case unknown

An unknown battery-charging state.

case unplugged

The device is not connected to a charger and is running on battery power.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Reading Information About the Battery

var isBatteryMonitoringEnabled: Bool

A Boolean value that determines whether the app can monitor the device’s battery.

var batteryLevel: Float

The battery’s current percent charge.

var batteryState: WKInterfaceDeviceBatteryState

The device’s battery state.

