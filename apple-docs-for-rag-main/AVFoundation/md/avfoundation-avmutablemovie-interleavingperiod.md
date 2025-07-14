

- AVFoundation
- AVMutableMovie
-  interleavingPeriod 

Instance Property

# interleavingPeriod

A time period indicating the duration for interleaving runs of samples for each track.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
var interleavingPeriod: CMTime { get set }
```

## Discussion

Default value is `0.5` seconds.

## See Also

### Configuring a Movie

var isModified: Bool

A Boolean value that indicates whether the movie is in a modified state.

var timescale: CMTimeScale

The time scale of the movie.

var defaultMediaDataStorage: AVMediaDataStorage?

The default storage container for media data that you add to a movie.

