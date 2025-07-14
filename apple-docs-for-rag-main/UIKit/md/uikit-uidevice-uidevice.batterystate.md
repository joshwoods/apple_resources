

- UIKit
- UIDevice
-  UIDevice.BatteryState 

Enumeration

# UIDevice.BatteryState

Constants that describe the battery power state of the device.

iOSiPadOSMac CatalystvisionOS

``` source
enum BatteryState
```

## Overview

These constants are used by the batteryState property.

## Topics

### Constants

case unknown

The battery state for the device can’t be determined.

case unplugged

The device isn’t plugged into power; the battery is discharging.

case charging

The device is plugged into power and the battery is less than 100% charged.

case full

The device is plugged into power and the battery is 100% charged.

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

### Getting the device battery state

var batteryLevel: Float

The battery charge level for the device.

var isBatteryMonitoringEnabled: Bool

A Boolean value that indicates whether battery monitoring is enabled.

var batteryState: UIDevice.BatteryState

The battery state for the device.

