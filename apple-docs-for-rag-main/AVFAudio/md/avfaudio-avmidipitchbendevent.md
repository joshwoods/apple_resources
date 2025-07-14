

- AVFAudio
-  AVMIDIPitchBendEvent 

Class

# AVMIDIPitchBendEvent

An object that represents a MIDI pitch bend message.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
class AVMIDIPitchBendEvent
```

## Topics

### Creating a Pitch Bend Event

init(channel: UInt32, value: UInt32)

Creates an event with a channel and pitch bend value.

### Configuring a Pitch Bend Event

var value: UInt32

The value of the pitch bend event.

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

class AVMIDIPolyPressureEvent

An object that represents a MIDI poly or key pressure event.

class AVMIDIControlChangeEvent

An object that represents a MIDI control change message.

