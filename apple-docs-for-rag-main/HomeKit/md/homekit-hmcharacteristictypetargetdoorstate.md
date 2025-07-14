

- HomeKit
-  HMCharacteristicTypeTargetDoorState 

Global Variable

# HMCharacteristicTypeTargetDoorState

The target door state.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+tvOS 10.0+visionOS 1.0+watchOS 2.0+

``` source
let HMCharacteristicTypeTargetDoorState: String
```

## Discussion

The corresponding value is one of the constants in the HMCharacteristicValueDoorState enumeration.

Doors take time to move between states, so the target door state may not match the current door state at a given moment in time.

## Topics

### Values

enum HMCharacteristicValueDoorState

Possible values for the state of a door.

enum HMCharacteristicValueTargetDoorState

Values that indicate the state of a door.

## See Also

### Doors and windows

let HMCharacteristicTypeCurrentDoorState: String

The current door state.

let HMCharacteristicTypeCurrentPosition: String

The current position of a door, window, awning, or window covering.

let HMCharacteristicTypeTargetPosition: String

The target position of a door, window, awning, or window covering.

let HMCharacteristicTypePositionState: String

The position of an accessory like a door, window, awning, or window covering.

let HMCharacteristicTypeStatusJammed: String

An indicator of whether an accessory is jammed.

let HMCharacteristicTypeHoldPosition: String

A control for holding the position of an accessory like a door or window.

let HMCharacteristicTypeSlatType: String

The type of slat on an accessory like a window or a fan.

let HMCharacteristicTypeCurrentSlatState: String

The current state of slats on an accessory like a window or a fan.

