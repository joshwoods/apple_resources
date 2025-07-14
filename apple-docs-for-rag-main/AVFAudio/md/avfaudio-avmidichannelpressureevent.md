

- AVFAudio
-  AVMIDIChannelPressureEvent 

Class

# AVMIDIChannelPressureEvent

An object that represents a MIDI channel pressure message.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
class AVMIDIChannelPressureEvent
```

## Overview

The effect of this message depends on the AVMusicTrack destination audio unit, and the capabilities of the destination’s loaded instrument.

## Topics

### Creating a Pressure Event

init(channel: UInt32, pressure: UInt32)

Creates a pressure event with a channel and pressure value.

### Configuring a Pressure Event

var pressure: UInt32

The MIDI channel pressure.

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

class AVMIDIProgramChangeEvent

An object that represents a MIDI program or patch change message.

class AVMIDIPolyPressureEvent

An object that represents a MIDI poly or key pressure event.

class AVMIDIPitchBendEvent

An object that represents a MIDI pitch bend message.

class AVMIDIControlChangeEvent

An object that represents a MIDI control change message.

