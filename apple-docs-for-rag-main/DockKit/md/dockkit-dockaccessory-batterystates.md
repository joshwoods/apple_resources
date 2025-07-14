

- DockKit
- DockAccessory
-  batteryStates 

Instance Property

# batteryStates

Battery states from the accessory that indicate changes in battery charge or readiness

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
final var batteryStates: DockAccessory.BatteryStates { get throws }
```

## Return Value

Accessory events related to button presses and common camera controls.

## Discussion

Throws

DockKitError.notConnected if device is disconnected, or DockKitError.notSupportedByDevice if device doesn’t support updates.

