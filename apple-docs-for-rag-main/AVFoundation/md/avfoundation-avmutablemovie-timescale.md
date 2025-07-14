

- AVFoundation
- AVMutableMovie
-  timescale 

Instance Property

# timescale

The time scale of the movie.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
var timescale: CMTimeScale { get set }
```

## Discussion

The default movie time scale is `600`. In certain cases, you may want to set this to a different value. For example, a movie that contains a single audio track should set the movie time scale to the media time scale of that track. Set the value of this property on a new empty movie before you perform any edits on it.

## See Also

### Configuring a Movie

var isModified: Bool

A Boolean value that indicates whether the movie is in a modified state.

var interleavingPeriod: CMTime

A time period indicating the duration for interleaving runs of samples for each track.

var defaultMediaDataStorage: AVMediaDataStorage?

The default storage container for media data that you add to a movie.

