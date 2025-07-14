

- Audio Toolbox
-  MusicTrackGetProperty(\_:\_:\_:\_:) 

Function

# MusicTrackGetProperty(\_:\_:\_:\_:)

Gets a music track property value.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+

``` source
func MusicTrackGetProperty(
    _ inTrack: MusicTrack,
    _ inPropertyID: UInt32,
    _ outData: UnsafeMutableRawPointer,
    _ ioLength: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`inTrack`  

The music track that you want to get a property value from.

`inPropertyID`  

The identifier for the music track property that you want to get. See Music Track Properties for possible values.

`outData`  

On output, the requested property value.

`ioLength`  

On input, the available size for the retrieved property value. On output, the size of the valid property data that `outData` points to.

## Return Value

A result code.

## Discussion

Music track property values are always accessed by reference. As of OS X v10.6, all such property values are fixed length.

This function’s main purpose is to retrieve a music track property value, but you also use it to obtain the size of a variable-length property. Do this, prior to retrieving a variable-length property value, to ensure that you allocate enough memory in `outData` to hold the value.

To obtain a property value’s size, call this function with the `outData` parameter set to `NULL`. On output, the `ioLength` parameter contains the property size.

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

