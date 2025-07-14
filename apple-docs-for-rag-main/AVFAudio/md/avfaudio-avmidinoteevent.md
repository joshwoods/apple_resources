

- AVFAudio
-  AVMIDINoteEvent 

Class

# AVMIDINoteEvent

An object that represents MIDI note on or off messages.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
class AVMIDINoteEvent
```

## Topics

### Creating a MIDI Note Event

init(channel: UInt32, key: UInt32, velocity: UInt32, duration: AVMusicTimeStamp)

Creates an event with a MIDI channel, key number, velocity, and duration.

### Configuring a MIDI Note Event

var channel: UInt32

The MIDI channel.

var key: UInt32

The MIDI key number.

var velocity: UInt32

The MIDI velocity.

var duration: AVMusicTimeStamp

The duration for the note, in beats.

## Relationships

### Inherits From

- AVMusicEvent

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Handling MIDI Events

class AVMIDIMetaEvent

An object that represents MIDI meta event messages.

class AVMIDISysexEvent

An object that represents a MIDI system exclusive message.

