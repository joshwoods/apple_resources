

- AVFoundation
- AVAssetWriter
-  initialMovieFragmentSequenceNumber 

Instance Property

# initialMovieFragmentSequenceNumber

The sequence number of the initial movie fragment.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var initialMovieFragmentSequenceNumber: Int { get set }
```

## Discussion

If you combine movie fragments that you create from multiple asset writers, movie fragment sequence numbers need to increase monotonically across the entire combined collection, in temporal order. The default value of this property is `1`.

You can’t set this property after writing starts.

## See Also

### Configuring Fragment Output

var movieFragmentInterval: CMTime

The interval at which to write movie fragments.

var initialMovieFragmentInterval: CMTime

The interval at which to write the initial movie fragment.

var producesCombinableFragments: Bool

A Boolean value that indicates whether the asset writer outputs movie fragments suitable for combining with others.

var overallDurationHint: CMTime

A hint of the final duration of the output file.

var movieTimeScale: CMTimeScale

The time scale of the movie.

