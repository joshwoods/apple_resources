

- AVFAudio
- AVMusicTrack
-  numberOfLoops 

Instance Property

# numberOfLoops

The number of times the track’s loop repeats.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var numberOfLoops: Int { get set }
```

## Discussion

Use the value AVMusicTrackLoopCount.forever to loop the track forever. Otherwise, valid values start at `1`.

## See Also

### Configuring the Looping State

var isLoopingEnabled: Bool

A Boolean value that indicates whether the track is in a looping state.

var loopRange: AVBeatRange

The timestamp range for the loop, in beats.

