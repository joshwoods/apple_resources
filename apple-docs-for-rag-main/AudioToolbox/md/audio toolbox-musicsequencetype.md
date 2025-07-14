

- Audio Toolbox
-  MusicSequenceType 

Enumeration

# MusicSequenceType

The various types of music sequences.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
enum MusicSequenceType
```

## Topics

### Constants

case beats

Used for a music sequence that corresponds to a normal MIDI file. The tempo track defines the number of beats per second and can have multiple tempo events.

case seconds

Used for a music sequence that corresponds to a MIDI file, but employs SMPTE timecode. The tempo track contains a single tempo event that specifies 60 beat-per-minute.

case samples

Used for audio samples; a music sequence of this type cannot be saved to a MIDI file. The tempo track contains a single tempo event that specifies an audio sample rate in samples-per-second.

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

