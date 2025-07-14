

- HomeKit
-  HMCharacteristicTypeHoldPosition 

Global Variable

# HMCharacteristicTypeHoldPosition

A control for holding the position of an accessory like a door or window.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
let HMCharacteristicTypeHoldPosition: String
```

## Discussion

The corresponding value is a write-only Boolean. Write a value of `true` to indicate that the current position should be maintained. The accessory ignores a written value of `false`. Write a value to the HMCharacteristicTypeTargetPosition characteristic to release the hold.

## See Also

### Doors and windows

let HMCharacteristicTypeCurrentDoorState: String

The current door state.

let HMCharacteristicTypeTargetDoorState: String

The target door state.

let HMCharacteristicTypeCurrentPosition: String

The current position of a door, window, awning, or window covering.

let HMCharacteristicTypeTargetPosition: String

The target position of a door, window, awning, or window covering.

let HMCharacteristicTypePositionState: String

The position of an accessory like a door, window, awning, or window covering.

let HMCharacteristicTypeStatusJammed: String

An indicator of whether an accessory is jammed.

let HMCharacteristicTypeSlatType: String

The type of slat on an accessory like a window or a fan.

let HMCharacteristicTypeCurrentSlatState: String

The current state of slats on an accessory like a window or a fan.

