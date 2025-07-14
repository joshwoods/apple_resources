

- Audio Toolbox
-  MusicSequenceSetSequenceType(\_:\_:) 

Function

# MusicSequenceSetSequenceType(\_:\_:)

Sets the sequence type for a music sequence.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func MusicSequenceSetSequenceType(
    _ inSequence: MusicSequence,
    _ inType: MusicSequenceType
) -> OSStatus
```

## Parameters 

`inSequence`  

The music sequence whose sequence type you want to set.

`inType`  

The type of sequence to assign to the music sequence. For the list of available sequence types, see MusicSequenceType. The default sequence type is `kMusicSequenceType_Beats`.

## Return Value

A result code.

## Discussion

The sequence type can be set to `kMusicSequenceType_Beats` at any time. The sequence type can only be set to `kMusicSequenceType_Seconds` or `kMusicSequenceType_Samples` if there are no tempo events already in the sequence.

The following considerations pertain to the various sequence types:

- `kMusicSequenceType_Beats`—Tempo is specified as beats-per-minute. A music sequence of this type can contain any number of tempo events.

- `kMusicSequenceType_Samples`—Tempo is specified as a sample rate, in terms of samples-per-second. If you set the tempo to 44,100 using a sequence of this type, then 44,100 beats corresponds to a duration of one second.

- `kMusicSequenceType_Seconds`—The tempo should be set to 60; a beat is a second.

After setting a music sequence to the `kMusicSequenceType_Samples` or `kMusicSequenceType_Seconds` type, add a single tempo event to specify the tempo.

A meta event of interest for the `kMusicSequenceType_Seconds` sequence type is the SMPTE Offset meta event, which is stored in the tempo track. The sequence doesn’t do anything with this event.

## See Also

### Managing Music Sequences

func NewMusicSequence(UnsafeMutablePointer&lt;MusicSequence?>) -> OSStatus

Creates a new empty music sequence.

func DisposeMusicSequence(MusicSequence) -> OSStatus

Disposes of a music sequence.

func MusicSequenceBarBeatTimeToBeats(MusicSequence, UnsafePointer&lt;CABarBeatTime>, UnsafeMutablePointer&lt;MusicTimeStamp>) -> OSStatus

Formats a music sequence’s bar-beat time to its beat time.

func MusicSequenceBeatsToBarBeatTime(MusicSequence, MusicTimeStamp, UInt32, UnsafeMutablePointer&lt;CABarBeatTime>) -> OSStatus

Formats a music sequence’s beat time to its bar-beat time.

func MusicSequenceDisposeTrack(MusicSequence, MusicTrack) -> OSStatus

Removes a music track from a music sequence, and disposes of the track.

func MusicSequenceFileCreate(MusicSequence, CFURL, MusicSequenceFileTypeID, MusicSequenceFileFlags, Int16) -> OSStatus

Creates a MIDI file from the events in a music sequence.

func MusicSequenceFileCreateData(MusicSequence, MusicSequenceFileTypeID, MusicSequenceFileFlags, Int16, UnsafeMutablePointer&lt;Unmanaged&lt;CFData>?>) -> OSStatus

Creates a data object containing the events from a music sequence.

func MusicSequenceFileLoad(MusicSequence, CFURL, MusicSequenceFileTypeID, MusicSequenceLoadFlags) -> OSStatus

Loads data into a music sequence from a URL reference.

func MusicSequenceFileLoadData(MusicSequence, CFData, MusicSequenceFileTypeID, MusicSequenceLoadFlags) -> OSStatus

Load data into a music sequence from a data reference.

func MusicSequenceGetAUGraph(MusicSequence, UnsafeMutablePointer&lt;AUGraph?>) -> OSStatus

Gets the audio processing graph associated with a music sequence.

func MusicSequenceGetBeatsForSeconds(MusicSequence, Float64, UnsafeMutablePointer&lt;MusicTimeStamp>) -> OSStatus

Calculates the number of beats that correspond to a number of seconds.

func MusicSequenceGetIndTrack(MusicSequence, UInt32, UnsafeMutablePointer&lt;MusicTrack?>) -> OSStatus

Gets the music track at the specified track index.

func MusicSequenceGetInfoDictionary(MusicSequence) -> CFDictionary

Returns a dictionary containing music sequence information.

func MusicSequenceGetSMPTEResolution(Int16, UnsafeMutablePointer&lt;Int8>, UnsafeMutablePointer&lt;UInt8>)

func MusicSequenceGetSecondsForBeats(MusicSequence, MusicTimeStamp, UnsafeMutablePointer&lt;Float64>) -> OSStatus

Calculates the number of seconds that correspond to a number of beats.

