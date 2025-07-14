

- AVFAudio
-  AVMIDIPolyPressureEvent 

Class

# AVMIDIPolyPressureEvent

An object that represents a MIDI poly or key pressure event.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
class AVMIDIPolyPressureEvent
```

## Topics

### Creating a Poly Pressure Event

init(channel: UInt32, key: UInt32, pressure: UInt32)

Creates an event with a channel, MIDI key number, and a key pressure value.

### Configuring a Poly Pressure Event

var key: UInt32

The MIDI key number.

var pressure: UInt32

The poly pressure value for the requested key.

## Relationships

### Inherits From

- AVMIDIChannelEvent

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Handling MIDI Channel Events

class AVMIDIChannelEvent

A base class for all MIDI messages that operate on a single MIDI channel.

class AVMIDIChannelPressureEvent

An object that represents a MIDI channel pressure message.

class AVMIDIProgramChangeEvent

An object that represents a MIDI program or patch change message.

class AVMIDIPitchBendEvent

An object that represents a MIDI pitch bend message.

class AVMIDIControlChangeEvent

An object that represents a MIDI control change message.

