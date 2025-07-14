

- AVFAudio
-  AVExtendedTempoEvent 

Class

# AVExtendedTempoEvent

An object that represents a tempo change to a specific beats-per-minute value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
class AVExtendedTempoEvent
```

## Topics

### Creating a Tempo Event

init(tempo: Double)

Creates an extended tempo event.

### Configuring a Tempo Event

var tempo: Double

The tempo in beats per minute as a positive value.

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

class AVMusicUserEvent

An object that represents a custom user message.

class AVParameterEvent

An object that represents a parameter event on a music track’s destination.

class AVAUPresetEvent

An object that represents a preset load and change on the music track’s destination audio unit.

class AVExtendedNoteOnEvent

An object that represents a custom extension of a MIDI note on event.

