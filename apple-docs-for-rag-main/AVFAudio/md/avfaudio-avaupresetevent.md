

- AVFAudio
-  AVAUPresetEvent 

Class

# AVAUPresetEvent

An object that represents a preset load and change on the music track’s destination audio unit.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
class AVAUPresetEvent
```

## Topics

### Creating a Preset Event

init(scope: UInt32, element: UInt32, dictionary: [AnyHashable : Any])

Creates an event with the scope, element, and dictionary for the preset.

### Configuring a Preset Event

var scope: UInt32

The audio unit scope.

var element: UInt32

The element index in the scope.

var presetDictionary: [AnyHashable : Any]

The dictionary that contains the preset.

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

class AVExtendedTempoEvent

An object that represents a tempo change to a specific beats-per-minute value.

class AVExtendedNoteOnEvent

An object that represents a custom extension of a MIDI note on event.

