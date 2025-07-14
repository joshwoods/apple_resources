

- Audio Toolbox
- Music Player
-  Music Track Properties 

API Collection

# Music Track Properties

Properties for music tracks.

## Topics

### Constants

var kSequenceTrackProperty_LoopInfo: UInt32

Looping information for a music track.

var kSequenceTrackProperty_OffsetTime: UInt32

A music track’s start time in terms of beat number.

var kSequenceTrackProperty_MuteStatus: UInt32

The mute/unmute state of a music track. By default this value is `false` (not muted). A read/write Boolean value.

var kSequenceTrackProperty_SoloStatus: UInt32

The solo/unsolo state of a music track. By default this value is `false` (not soloed). A read/write Boolean value.

var kSequenceTrackProperty_AutomatedParameters: UInt32

Indicates whether or not a music track’s purpose is audio unit parameter automation. If this property’s value is other than 0, music events in the track can only indicate points in an automation curve. A read/write `UInt32` value, where a value other than 0 indicates that the track is for parameter automation.

var kSequenceTrackProperty_TrackLength: UInt32

The time of the last music event in a music track, plus time required for note fade-outs and so on.

var kSequenceTrackProperty_TimeResolution: UInt32

The time resolution for a sequence of music events. For example, this value can indicate the time resolution that was specified by the MIDI file used to construct a sequence.

## See Also

### Enumerations

Music Instrument Audio Unit Subtypes

struct MusicSequenceFileFlags

Flags that configure the behavior of the MusicSequenceFileCreate(_:_:_:_:_:) and MusicSequenceFileCreateData(_:_:_:_:_:) functions.

enum MusicSequenceFileTypeID

The various types of files that can be parsed by a music sequence.

struct MusicSequenceLoadFlags

Flags used to configure the behavior of the MusicSequenceFileLoad(_:_:_:_:) and MusicSequenceFileLoadData(_:_:_:_:) functions.

enum MusicSequenceType

The various types of music sequences.

Music Extended Control Event Type

Music Player Errors

Music Event Types

Music Note Events

Music Device Selectors

Music Device Properties

Music Device Sample Frame Mask

Music Device Unit Properties

Instrument Types

Music Device Generic Properties

