

- Game Controller
-  GCRacingWheelInput 

Class

# GCRacingWheelInput

A controller profile that supports a racing wheel.

Mac Catalyst 16.0+macOS 13.0+

``` source
class GCRacingWheelInput
```

## Mentioned in 

Handling input events

## Topics

### Creating snapshots

func capture() -> GCRacingWheelInputState

Returns a snapshot of the racing wheel inputs.

### Polling for input

func nextInputState() -> (any GCRacingWheelInputState &amp; GCDevicePhysicalInputStateDiff)?

Returns the next input state of the racing wheel from the queue.

## Relationships

### Inherits From

- GCRacingWheelInputState

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- GCDevicePhysicalInput
- GCDevicePhysicalInputState
- Hashable
- NSObjectProtocol

## See Also

### Racing wheel input

class GCRacingWheelInputState

The input for the wheel of a racing wheel controller.

