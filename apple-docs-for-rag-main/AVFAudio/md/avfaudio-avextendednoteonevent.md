

- AVFAudio
-  AVExtendedNoteOnEvent 

Class

# AVExtendedNoteOnEvent

An object that represents a custom extension of a MIDI note on event.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
class AVExtendedNoteOnEvent
```

## Overview

Use this to allow an app to trigger a custom note on event on one of several Apple audio units that support it. The floating point note and velocity numbers allow for optional fractional control of the note’s runtime properties that the system modulates by those inputs. This event supports the possibility of an audio unit with more than the standard 16 MIDI channels.

## Topics

### Creating a Note On Event

init(midiNote: Float, velocity: Float, groupID: UInt32, duration: AVMusicTimeStamp)

Creates an event with a MIDI note, velocity, group identifier, and duration.

init(midiNote: Float, velocity: Float, instrumentID: UInt32, groupID: UInt32, duration: AVMusicTimeStamp)

Creates a note on event with the default instrument.

### Configuring a Note On Event

var midiNote: Float

The MIDI note number.

var velocity: Float

The MDI velocity.

var instrumentID: UInt32

The instrument identifier.

var groupID: UInt32

The audio unit channel that handles the event.

var duration: AVMusicTimeStamp

The duration of the event, in beats.

### Getting the Default Instrument

class let defaultInstrument: UInt32

A constant that represents the default instrument identifier.

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

class AVExtendedTempoEvent

An object that represents a tempo change to a specific beats-per-minute value.

