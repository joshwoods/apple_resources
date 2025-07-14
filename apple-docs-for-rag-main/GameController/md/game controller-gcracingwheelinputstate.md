

- Game Controller
-  GCRacingWheelInputState 

Class

# GCRacingWheelInputState

The input for the wheel of a racing wheel controller.

Mac Catalyst 16.0+macOS 13.0+

``` source
class GCRacingWheelInputState
```

## Topics

### Getting input elements

var wheel: GCSteeringWheelElement

The controller’s wheel element.

var acceleratorPedal: (any GCButtonElement)?

The controller’s accelerator pedal element.

var brakePedal: (any GCButtonElement)?

The controller’s brake pedal element.

var clutchPedal: (any GCButtonElement)?

The controller’s clutch element.

var shifter: GCGearShifterElement?

The controller’s gear shift element.

### Accessing elements by name

var GCInputSteeringWheel: String

The name of the steering wheel element.

var GCInputShifter: String

The name of the shifter element.

var GCInputPedalClutch: String

The name of the clutch element.

var GCInputPedalAccelerator: String

The name of the accelerator element.

var GCInputPedalBrake: String

The name of the brake element.

## Relationships

### Inherits From

- NSObject

### Inherited By

- GCRacingWheelInput

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- GCDevicePhysicalInputState
- Hashable
- NSObjectProtocol

## See Also

### Racing wheel input

class GCRacingWheelInput

A controller profile that supports a racing wheel.

