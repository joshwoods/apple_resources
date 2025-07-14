

- Core MIDI
-  MIDITransform 

Structure

# MIDITransform

The transformation of a single type of MIDI event.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct MIDITransform
```

## Topics

### Configuring a Transform

var param: Int16

An argument to the transformation method (see description of MIDITransformType).

var transform: MIDITransformType

The type of transformation to apply to the event values.

### Initializers

init()

init(transform: MIDITransformType, param: Int16)

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Transforming Values

struct MIDIValueMap

A custom lookup table to transform MIDI 7-bit values, as contained in note numbers, velocities, control values, and so on.

struct MIDIControlTransform

A structure that describes the transformation of MIDI control change events.

enum MIDITransformType

Values that specify the type of MIDI transformation.

enum MIDITransformControlType

A set of values that indicate how to interpret control numbers.

