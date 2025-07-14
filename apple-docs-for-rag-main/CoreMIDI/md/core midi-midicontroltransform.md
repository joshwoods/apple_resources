

- Core MIDI
-  MIDIControlTransform 

Structure

# MIDIControlTransform

A structure that describes the transformation of MIDI control change events.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct MIDIControlTransform
```

## Overview

A single parameters object may describe any number of transformations to control events. It’s important to order multiple transformations correctly: filter out, remap, and then alter values.

The system performs all transformations internally using 14-bit values, so when you perform an add, min, or max transform on a 7-bit control value, the parameter must be a 14-bit value. For example, to add 10 to a control value, the parameter must be (10 \

| Control | Function                                    |
|---------|---------------------------------------------|
| 32-63   | The least signifcant bit of 0-31.           |
| 6/38    | Data entry.                                 |
| 96, 97  | Data increment and decrement, respectively. |
| 98-101  | NRPN/RPN                                    |

## Topics

### Configuring a Control Transform

var controlType: MIDITransformControlType

The type of control specified by the control number.

var remappedControlType: MIDITransformControlType

The remapped control type.

var controlNumber: UInt16

The control number to affect.

var transform: MIDITransformType

The type of transformation to apply to the event values.

var param: Int16

An argument to the transformation method.

### Initializers

init()

init(controlType: MIDITransformControlType, remappedControlType: MIDITransformControlType, controlNumber: UInt16, transform: MIDITransformType, param: Int16)

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Transforming Values

struct MIDIValueMap

A custom lookup table to transform MIDI 7-bit values, as contained in note numbers, velocities, control values, and so on.

struct MIDITransform

The transformation of a single type of MIDI event.

enum MIDITransformType

Values that specify the type of MIDI transformation.

enum MIDITransformControlType

A set of values that indicate how to interpret control numbers.

