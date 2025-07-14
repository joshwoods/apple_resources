

- Core HID
- HIDUsage
-  HIDUsage.GameControlsUsage 

Enumeration

# HIDUsage.GameControlsUsage

macOS 15.0+

``` source
enum GameControlsUsage
```

## Topics

### Enumeration Cases

case bump

case flipper

case formFittingGamepad

case gameController3D

case gamepadFireOrJump

case gamepadTrigger

case gunAutomatic

case gunBolt

case gunBurst

case gunClip

case gunDevice

case gunSafety

case gunSelector

case gunSingleShot

case heightOfPOV

case leanForwardOrBackward

case leanRightOrLeft

case moveForwardOrBackward

case moveRightOrLeft

case moveUpOrDown

case newGame

case pinballDevice

case pitchForwardOrBackward

case player

case pointOfView

case rollRightOrLeft

case secondaryFlipper

case shootBall

case turnRightOrLeft

### Initializers

init?(rawValue: UInt16)

Creates a new instance with the specified raw value.

### Instance Properties

var rawValue: UInt16

The corresponding value of the raw type.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static let page: UInt16

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

