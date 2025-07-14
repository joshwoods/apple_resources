

- Core MIDI
-  MIDITransformControlType 

Enumeration

# MIDITransformControlType

A set of values that indicate how to interpret control numbers.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum MIDITransformControlType
```

## Topics

### Transform Control Types

case controlType_7Bit

A 7-bit control type.

case controlType_14Bit

A 14-bit control type.

case controlType_7BitRPN

A 7-bit Registered Parameter Number (RPN).

case controlType_14BitRPN

A 14-bit Registered Parameter Number (RPN).

case controlType_7BitNRPN

A 7-bit Nonregistered Parameter Number (RPN).

case controlType_14BitNRPN

A 14-bit Nonregistered Parameter Number (RPN).

### Initializers

init?(rawValue: UInt8)

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

enum MIDITransformType

Values that specify the type of MIDI transformation.

