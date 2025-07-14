

- AVFAudio
- AVAudioSequencer
-  data(withSMPTEResolution:error:) 

Instance Method

# data(withSMPTEResolution:error:)

Gets a data object that contains the events from the sequence.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func data(
    withSMPTEResolution SMPTEResolution: Int,
    error outError: NSErrorPointer
) -> Data
```

## Parameters 

`SMPTEResolution`  

The relationship between tick and quarter note for saving to a Standard MIDI File. Pass `0` to use the default.

`outError`  

On exit, if an error occurs, a description of the error.

## Discussion

The client controls the lifetime of the data value this method returns.

## See Also

### Getting Sequence Properties

var isPlaying: Bool

A Boolean value that indicates whether the sequencer’s player is in a playing state.

var rate: Float

The playback rate of the sequencer’s player.

var tracks: [AVMusicTrack]

An array that contains all the tracks in the sequence.

var currentPositionInBeats: TimeInterval

The current playback position, in beats.

var currentPositionInSeconds: TimeInterval

The current playback position, in seconds.

var tempoTrack: AVMusicTrack

The track that contains tempo information about the sequence.

var userInfo: [String : Any]

A dictionary that contains metadata from a sequence.

struct InfoDictionaryKey

Constants that defines metadata keys for a sequencer.

var AVMusicTimeStampEndOfTrack: Double

A timestamp you use to access all events in a music track through a beat range.

