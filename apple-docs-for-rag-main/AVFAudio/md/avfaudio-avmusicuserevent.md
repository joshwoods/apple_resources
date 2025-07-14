

- AVFAudio
-  AVMusicUserEvent 

Class

# AVMusicUserEvent

An object that represents a custom user message.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
class AVMusicUserEvent
```

## Overview

When playback of an AVMusicTrack reaches this event, the system calls the track’s callback. You can’t modify the size and contents of an AVMusicUserEvent once you create it.

## Topics

### Creating a User Event

init(data: Data)

Creates a user event with the data you specify.

### Inspecting a User Event

var sizeInBytes: UInt32

The size of the data that the user event represents.

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

### Handling Music Events

class AVMusicEvent

A base class for the events you associate with a music track.

class AVParameterEvent

An object that represents a parameter event on a music track’s destination.

class AVAUPresetEvent

An object that represents a preset load and change on the music track’s destination audio unit.

class AVExtendedTempoEvent

An object that represents a tempo change to a specific beats-per-minute value.

class AVExtendedNoteOnEvent

An object that represents a custom extension of a MIDI note on event.

