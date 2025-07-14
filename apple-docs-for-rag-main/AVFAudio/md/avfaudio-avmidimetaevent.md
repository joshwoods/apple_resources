

- AVFAudio
-  AVMIDIMetaEvent 

Class

# AVMIDIMetaEvent

An object that represents MIDI meta event messages.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
class AVMIDIMetaEvent
```

## Overview

You can’t modify the size and contents of this event once you create it. This doesn’t verify that the content matches the MIDI specification.

You can only add AVMIDIMetaEvent.EventType.tempo, AVMIDIMetaEvent.EventType.smpteOffset, or AVMIDIMetaEvent.EventType.timeSignature to a sequence’s tempo track.

## Topics

### Creating a Meta Event

init(type: AVMIDIMetaEvent.EventType, data: Data)

Creates an event with a MIDI meta event type and data.

### Getting the Meta Event Type

var type: AVMIDIMetaEvent.EventType

The type of meta event.

enum EventType

Constants that represent the types of meta events.

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

class AVMIDINoteEvent

An object that represents MIDI note on or off messages.

class AVMIDISysexEvent

An object that represents a MIDI system exclusive message.

