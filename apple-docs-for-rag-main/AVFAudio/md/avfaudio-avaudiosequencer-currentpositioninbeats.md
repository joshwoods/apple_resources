

- AVFAudio
- AVAudioSequencer
-  currentPositionInBeats 

Instance Property

# currentPositionInBeats

The current playback position, in beats.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var currentPositionInBeats: TimeInterval { get set }
```

## Discussion

Setting this property positions the sequencer’s player to the specified beat. You can update this property while the player is in a playing state, in which case, playback resumes at the new position.

## See Also

### Getting Sequence Properties

var isPlaying: Bool

A Boolean value that indicates whether the sequencer’s player is in a playing state.

var rate: Float

The playback rate of the sequencer’s player.

var tracks: [AVMusicTrack]

An array that contains all the tracks in the sequence.

var currentPositionInSeconds: TimeInterval

The current playback position, in seconds.

var tempoTrack: AVMusicTrack

The track that contains tempo information about the sequence.

var userInfo: [String : Any]

A dictionary that contains metadata from a sequence.

struct InfoDictionaryKey

Constants that defines metadata keys for a sequencer.

func data(withSMPTEResolution: Int, error: NSErrorPointer) -> Data

Gets a data object that contains the events from the sequence.

var AVMusicTimeStampEndOfTrack: Double

A timestamp you use to access all events in a music track through a beat range.

