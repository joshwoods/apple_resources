

- Audio Toolbox
-  MusicSequenceBeatsToBarBeatTime(\_:\_:\_:\_:) 

Function

# MusicSequenceBeatsToBarBeatTime(\_:\_:\_:\_:)

Formats a music sequence’s beat time to its bar-beat time.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func MusicSequenceBeatsToBarBeatTime(
    _ inSequence: MusicSequence,
    _ inBeats: MusicTimeStamp,
    _ inSubbeatDivisor: UInt32,
    _ outBarBeatTime: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`inSequence`  

The music sequence that you want bar-beat time for.

`inBeats`  

The beats to be represented as bar-beats.

`inSubbeatDivisor`  

The denominator of the fractional number of beats.

`outBarBeatTime`  

On output, the music sequence’s bar-beat time.

## Return Value

A result code.

## Discussion

The sequence’s tempo track time signature events are used to calculate the bar-beat representation. If there are no Time Sig events added to the sequence 4/4 is assumed. A time signature event is a MIDI Meta Event as specified for MIDI files.

Refer to `AudioToolbox/CAClock.h` for more information.

## See Also

### Managing Music Sequences

func NewMusicSequence(UnsafeMutablePointer&lt;MusicSequence?>) -> OSStatus

Creates a new empty music sequence.

func DisposeMusicSequence(MusicSequence) -> OSStatus

Disposes of a music sequence.

func MusicSequenceBarBeatTimeToBeats(MusicSequence, UnsafePointer&lt;CABarBeatTime>, UnsafeMutablePointer&lt;MusicTimeStamp>) -> OSStatus

Formats a music sequence’s bar-beat time to its beat time.

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

func MusicSequenceGetSequenceType(MusicSequence, UnsafeMutablePointer&lt;MusicSequenceType>) -> OSStatus

Gets the sequence type for a music sequence.

