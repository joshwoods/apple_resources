

- AVFAudio
-  AVMIDIProgramChangeEvent 

Class

# AVMIDIProgramChangeEvent

An object that represents a MIDI program or patch change message.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
class AVMIDIProgramChangeEvent
```

## Overview

The effect of this message depends on the AVMusicTrack destination audio unit.

## Topics

### Creating a Program Change Event

init(channel: UInt32, programNumber: UInt32)

Creates a program change event with a channel and program number.

### Configuring a Program Change Event

var programNumber: UInt32

The MIDI program number.

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

class AVMIDIPolyPressureEvent

An object that represents a MIDI poly or key pressure event.

class AVMIDIPitchBendEvent

An object that represents a MIDI pitch bend message.

class AVMIDIControlChangeEvent

An object that represents a MIDI control change message.

