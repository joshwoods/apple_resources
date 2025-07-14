

- AVFoundation
- AVMutableMovie
-  isModified 

Instance Property

# isModified

A Boolean value that indicates whether the movie is in a modified state.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
var isModified: Bool { get set }
```

## Discussion

The value is true if you’ve modified the movie since you created it, saved it, or had its modified state cleared.

## See Also

### Configuring a Movie

var timescale: CMTimeScale

The time scale of the movie.

var interleavingPeriod: CMTime

A time period indicating the duration for interleaving runs of samples for each track.

var defaultMediaDataStorage: AVMediaDataStorage?

The default storage container for media data that you add to a movie.

