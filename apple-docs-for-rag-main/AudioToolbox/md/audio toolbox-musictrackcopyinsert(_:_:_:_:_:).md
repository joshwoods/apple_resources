

- Audio Toolbox
-  MusicTrackCopyInsert(\_:\_:\_:\_:\_:) 

Function

# MusicTrackCopyInsert(\_:\_:\_:\_:\_:)

Copies a range of events from one music track and inserts them into another music track.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+

``` source
func MusicTrackCopyInsert(
    _ inSourceTrack: MusicTrack,
    _ inSourceStartTime: MusicTimeStamp,
    _ inSourceEndTime: MusicTimeStamp,
    _ inDestTrack: MusicTrack,
    _ inDestInsertTime: MusicTimeStamp
) -> OSStatus
```

## Parameters 

`inSourceTrack`  

The music track that you want to copy events from.

`inSourceStartTime`  

The start time, in beats, for the range of music track events that you want to copy from the source track.

`inSourceEndTime`  

The end time, in beats, for the range of music track events that you want to copy from the source track.

`inDestTrack`  

The music track that you want to add events to.

`inDestInsertTime`  

The insertion point, in beats, in the destination music track for the copied events.

## Return Value

A result code.

## Discussion

The events in the destination music track, starting at the insertion point, are pushed later in time (that is, away from the start of the track) to make room for the inserted events.

The `inSourceStartTime` value must be less than the `inSourceEndTime` value.

## See Also

### Managing Music Tracks

func MusicTrackClear(MusicTrack, MusicTimeStamp, MusicTimeStamp) -> OSStatus

Removes a specified range of music track events.

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

func MusicTrackNewMetaEvent(MusicTrack, MusicTimeStamp, UnsafePointer&lt;MIDIMetaEvent>) -> OSStatus

Adds an event of type `MIDIMetaEvent` to a music track.

