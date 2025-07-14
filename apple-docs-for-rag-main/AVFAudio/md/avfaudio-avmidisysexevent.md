

- AVFAudio
-  AVMIDISysexEvent 

Class

# AVMIDISysexEvent

An object that represents a MIDI system exclusive message.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
class AVMIDISysexEvent
```

## Overview

You can’t modify the size and contents of this event once you create it.

## Topics

### Creates a System Event

init(data: Data)

Creates a system event with the data you specify.

### Getting the Size of the Event

var sizeInBytes: UInt32

The size of the data that this event contains.

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

class AVMIDIMetaEvent

An object that represents MIDI meta event messages.

