

- Audio Toolbox
-  MIDIMetaEvent 

Structure

# MIDIMetaEvent

Describes a MIDI metaevent such as lyric text, time signature, and so on.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct MIDIMetaEvent
```

## Topics

### Initializers

init()

init(metaEventType: UInt8, unused1: UInt8, unused2: UInt8, unused3: UInt8, dataLength: UInt32, data: UInt8)

### Instance Properties

var data: UInt8

var dataLength: UInt32

var metaEventType: UInt8

An integer that designates one of the types of MIDI metaevents.

var unused1: UInt8

var unused2: UInt8

var unused3: UInt8

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Managing Music Tracks

func MusicTrackClear(MusicTrack, MusicTimeStamp, MusicTimeStamp) -> OSStatus

Removes a specified range of music track events.

func MusicTrackCopyInsert(MusicTrack, MusicTimeStamp, MusicTimeStamp, MusicTrack, MusicTimeStamp) -> OSStatus

Copies a range of events from one music track and inserts them into another music track.

func MusicTrackCut(MusicTrack, MusicTimeStamp, MusicTimeStamp) -> OSStatus

Removes a specified range of music track events, and shifts later events toward the start of the track to fill in the gap.

func MusicTrackGetDestMIDIEndpoint(MusicTrack, UnsafeMutablePointer&lt;MIDIEndpointRef>) -> OSStatus

Gets the MIDI endpoint that is the event target for a music track.

func MusicTrackGetDestNode(MusicTrack, UnsafeMutablePointer&lt;AUNode>) -> OSStatus

Gets the audio unit node that is the event target for a music track.

func MusicTrackGetProperty(MusicTrack, UInt32, UnsafeMutableRawPointer, UnsafeMutablePointer&lt;UInt32>) -> OSStatus

Gets a music track property value.

func MusicTrackGetSequence(MusicTrack, UnsafeMutablePointer&lt;MusicSequence?>) -> OSStatus

Gets the music sequence that the music track is a member of.

func MusicTrackMerge(MusicTrack, MusicTimeStamp, MusicTimeStamp, MusicTrack, MusicTimeStamp) -> OSStatus

Copies a range of events from one music track and merges them into another music track.

func MusicTrackMoveEvents(MusicTrack, MusicTimeStamp, MusicTimeStamp, MusicTimeStamp) -> OSStatus

Shifts music track events forward or backward in time, in terms of beats.

func MusicTrackNewAUPresetEvent(MusicTrack, MusicTimeStamp, UnsafePointer&lt;AUPresetEvent>) -> OSStatus

Adds an event of type `AUPresetEvent` to a music track.

func MusicTrackNewExtendedNoteEvent(MusicTrack, MusicTimeStamp, UnsafePointer&lt;ExtendedNoteOnEvent>) -> OSStatus

Adds an event of type `ExtendedNoteOnEvent` to a music track.

func MusicTrackNewExtendedTempoEvent(MusicTrack, MusicTimeStamp, Float64) -> OSStatus

Adds a tempo to a music track.

func MusicTrackNewMIDIChannelEvent(MusicTrack, MusicTimeStamp, UnsafePointer&lt;MIDIChannelMessage>) -> OSStatus

Adds an event of type `MIDIChannelMessage` to a music track.

func MusicTrackNewMIDINoteEvent(MusicTrack, MusicTimeStamp, UnsafePointer&lt;MIDINoteMessage>) -> OSStatus

Adds an event of type `MIDINoteMessage` to a music track.

func MusicTrackNewMIDIRawDataEvent(MusicTrack, MusicTimeStamp, UnsafePointer&lt;MIDIRawData>) -> OSStatus

Adds an event of type `MIDIRawData` to a music track.

