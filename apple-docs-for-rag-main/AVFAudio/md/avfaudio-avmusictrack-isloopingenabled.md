

- AVFAudio
- AVMusicTrack
-  isLoopingEnabled 

Instance Property

# isLoopingEnabled

A Boolean value that indicates whether the track is in a looping state.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var isLoopingEnabled: Bool { get set }
```

## Discussion

If you don’t set loopRange, the framework loops the full track.

## See Also

### Configuring the Looping State

var loopRange: AVBeatRange

The timestamp range for the loop, in beats.

var numberOfLoops: Int

The number of times the track’s loop repeats.

