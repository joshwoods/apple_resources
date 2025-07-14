

- AVFAudio
-  AVMIDIChannelEvent 

Class

# AVMIDIChannelEvent

A base class for all MIDI messages that operate on a single MIDI channel.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
class AVMIDIChannelEvent
```

## Topics

### Configuring a Channel Event

var channel: UInt32

The MIDI channel.

## Relationships

### Inherits From

- AVMusicEvent

### Inherited By

- AVMIDIChannelPressureEvent
- AVMIDIControlChangeEvent
- AVMIDIPitchBendEvent
- AVMIDIPolyPressureEvent
- AVMIDIProgramChangeEvent

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Handling MIDI Channel Events

class AVMIDIChannelPressureEvent

An object that represents a MIDI channel pressure message.

class AVMIDIProgramChangeEvent

An object that represents a MIDI program or patch change message.

class AVMIDIPolyPressureEvent

An object that represents a MIDI poly or key pressure event.

class AVMIDIPitchBendEvent

An object that represents a MIDI pitch bend message.

class AVMIDIControlChangeEvent

An object that represents a MIDI control change message.

