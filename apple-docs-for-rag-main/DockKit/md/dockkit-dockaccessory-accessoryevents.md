

- DockKit
- DockAccessory
-  accessoryEvents 

Instance Property

# accessoryEvents

Events from the accessory that signify button presses or common camera controls.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+

``` source
final var accessoryEvents: DockAccessory.AccessoryEvents { get throws }
```

## Return Value

Accessory events related to button presses and common camera controls.

## Discussion

Throws

DockKitError.notConnected if device is disconnected, or DockKitError.notSupportedByDevice if device doesn’t support updates.

