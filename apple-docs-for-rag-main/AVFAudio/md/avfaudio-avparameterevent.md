

- AVFAudio
-  AVParameterEvent 

Class

# AVParameterEvent

An object that represents a parameter event on a music track’s destination.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
class AVParameterEvent
```

## Overview

When you configure an audio unit as the destination for an AVMusicTrack that contains this event, you can schedule and automate parameter changes.

When the track is playing as part of a sequence, the destination audio unit receives set-parameter messages whose values change smoothly along a linear ramp between each event’s beat location.

If you add an event to an empty, non-automation track, the track becomes an automation track.

## Topics

### Creating a Parameter Event

init(parameterID: UInt32, scope: UInt32, element: UInt32, value: Float)

Creates an event with a parameter identifier, scope, element, and value for the parameter to set.

### Configuring a Parameter Event

var parameterID: UInt32

The identifier of the parameter.

var scope: UInt32

The audio unit scope for the parameter.

var element: UInt32

The element index in the scope.

var value: Float

The value of the parameter to set.

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

class AVAUPresetEvent

An object that represents a preset load and change on the music track’s destination audio unit.

class AVExtendedTempoEvent

An object that represents a tempo change to a specific beats-per-minute value.

class AVExtendedNoteOnEvent

An object that represents a custom extension of a MIDI note on event.

