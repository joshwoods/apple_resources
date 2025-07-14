

- Audio Toolbox
-  MusicTrackMoveEvents(\_:\_:\_:\_:) 

Function

# MusicTrackMoveEvents(\_:\_:\_:\_:)

Shifts music track events forward or backward in time, in terms of beats.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+

``` source
func MusicTrackMoveEvents(
    _ inTrack: MusicTrack,
    _ inStartTime: MusicTimeStamp,
    _ inEndTime: MusicTimeStamp,
    _ inMoveTime: MusicTimeStamp
) -> OSStatus
```

## Parameters 

`inTrack`  

The track whose events you want to move forward or backward in time.

`inStartTime`  

The current start time, in beats, for the music track events you want to move.

`inEndTime`  

The current end time, in beats, for the music track events you want to move.

`inMoveTime`  

The number of beats to move the specified range of music track events. A positive value moves the events toward the end of the music track; a negative value moves the events toward the start.

## Return Value

A result code.

## Discussion

The `inStartTime` value must be less than the `inEndTime` value.

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

