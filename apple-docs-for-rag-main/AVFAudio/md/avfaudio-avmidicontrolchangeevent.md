

- AVFAudio
-  AVMIDIControlChangeEvent 

Class

# AVMIDIControlChangeEvent

An object that represents a MIDI control change message.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
class AVMIDIControlChangeEvent
```

## Topics

### Creating a Control Change Event

init(channel: UInt32, messageType: AVMIDIControlChangeEvent.MessageType, value: UInt32)

Creates an event with a channel, control change type, and a value.

### Inspecting a Control Change Event

var value: UInt32

The value of the control change event.

var messageType: AVMIDIControlChangeEvent.MessageType

The type of control change message.

enum MessageType

Constants that represents control change event types.

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

class AVMIDIPitchBendEvent

An object that represents a MIDI pitch bend message.

