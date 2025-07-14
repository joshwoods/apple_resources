

- AVFAudio
- AVMusicTrack
-  loopRange 

Instance Property

# loopRange

The timestamp range for the loop, in beats.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var loopRange: AVBeatRange { get set }
```

## Discussion

You set the loop by specifying its beat range.

## See Also

### Configuring the Looping State

var isLoopingEnabled: Bool

A Boolean value that indicates whether the track is in a looping state.

var numberOfLoops: Int

The number of times the track’s loop repeats.

