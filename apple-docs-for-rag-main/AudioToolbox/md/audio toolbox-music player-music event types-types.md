

- Audio Toolbox
- Music Player
-  Music Event Types 

API Collection

# Music Event Types

## Topics

### Constants

var kMusicEventType_AUPreset: UInt32

An event containing an audio unit user preset dictionary.

var kMusicEventType_ExtendedNote: UInt32

A non-MIDI music event with variable number of parameters.

var kMusicEventType_ExtendedTempo: UInt32

An event that signals a change in tempo, in beats-per-minute.

var kMusicEventType_MIDIChannelMessage: UInt32

A MIDI channel message, other than note control.

var kMusicEventType_MIDINoteMessage: UInt32

A MIDI note-on message, including duration.

var kMusicEventType_MIDIRawData: UInt32

MIDI system-exclusive data.

var kMusicEventType_Meta: UInt32

A standard MIDI file metaevent.

var kMusicEventType_NULL: UInt32

A null music event.

var kMusicEventType_Parameter: UInt32

An audio unit parameter event.

var kMusicEventType_User: UInt32

User-defined data.

## See Also

### Enumerations

Music Instrument Audio Unit Subtypes

Music Track Properties

Properties for music tracks.

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

Music Note Events

Music Device Selectors

Music Device Properties

Music Device Sample Frame Mask

Music Device Unit Properties

Instrument Types

Music Device Generic Properties

