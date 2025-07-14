

- Game Controller
- GCDeviceBattery
-  GCDeviceBattery.State 

Enumeration

# GCDeviceBattery.State

A state that indicates whether a device’s battery has power and is charging.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
enum State
```

## Topics

### States

case unknown

The state of the device’s battery is unknown.

case discharging

The device’s battery is discharging.

case charging

The device’s battery has power and is charging, but isn’t fully charged.

case full

The device’s battery has power and is fully charged.

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

### Getting the battery level and state

var batteryLevel: Float

The charge level of a device’s battery.

var batteryState: GCDeviceBattery.State

The state of a device’s battery.

