

- Core MIDI
-  MIDITransformType 

Enumeration

# MIDITransformType

Values that specify the type of MIDI transformation.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum MIDITransformType
```

## Topics

### Transform Types

case none

No transformation.

case filterOut

A transformation that filters out an event type.

case mapControl

A transformation that changes a specified control number to a supplied parameter value.

case add

A transform that adds a parameter value.

case scale

A transform that multiplies by the specified parameter value.

case minValue

A transform that sets the minimum value to the specified parameter value.

case maxValue

A transform that sets the maximum value to the specified parameter value.

case mapValue

A transform that maps one value to another.

### Initializers

init?(rawValue: UInt16)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Transforming Values

struct MIDIValueMap

A custom lookup table to transform MIDI 7-bit values, as contained in note numbers, velocities, control values, and so on.

struct MIDIControlTransform

A structure that describes the transformation of MIDI control change events.

struct MIDITransform

The transformation of a single type of MIDI event.

enum MIDITransformControlType

A set of values that indicate how to interpret control numbers.

