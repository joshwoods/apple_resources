

- AVFAudio
- AVAudioSequencer
-  tempoTrack 

Instance Property

# tempoTrack

The track that contains tempo information about the sequence.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var tempoTrack: AVMusicTrack { get }
```

## Discussion

Each sequence has a single tempo track. The framework places all tempo events into this track along with other appropriate events, such as the time signature from a MIDI file.

You can edit the tempo track like any other track. The framework ignores nontempo events in the track.

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

var userInfo: [String : Any]

A dictionary that contains metadata from a sequence.

struct InfoDictionaryKey

Constants that defines metadata keys for a sequencer.

func data(withSMPTEResolution: Int, error: NSErrorPointer) -> Data

Gets a data object that contains the events from the sequence.

var AVMusicTimeStampEndOfTrack: Double

A timestamp you use to access all events in a music track through a beat range.

