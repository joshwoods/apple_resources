

- Game Controller
- GCDeviceBattery
-  batteryLevel 

Instance Property

# batteryLevel

The charge level of a device’s battery.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var batteryLevel: Float { get }
```

## Discussion

The battery level is a percentage ranging from `0.0` (fully discharged) to `1.0` (100% charged). The default value for this property is `0.0`.

## See Also

### Getting the battery level and state

var batteryState: GCDeviceBattery.State

The state of a device’s battery.

enum State

A state that indicates whether a device’s battery has power and is charging.

