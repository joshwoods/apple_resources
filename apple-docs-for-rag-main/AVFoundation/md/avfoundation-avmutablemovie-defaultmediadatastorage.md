

- AVFoundation
- AVMutableMovie
-  defaultMediaDataStorage 

Instance Property

# defaultMediaDataStorage

The default storage container for media data that you add to a movie.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
@NSCopying
var defaultMediaDataStorage: AVMediaDataStorage? { get set }
```

## Discussion

This value specifies a location to write sample data that you add to a movie, for any track for whose mediaDataStorage property is `nil`.

## See Also

### Configuring a Movie

var isModified: Bool

A Boolean value that indicates whether the movie is in a modified state.

var timescale: CMTimeScale

The time scale of the movie.

var interleavingPeriod: CMTime

A time period indicating the duration for interleaving runs of samples for each track.

