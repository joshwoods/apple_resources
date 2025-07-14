

- AVFoundation
- AVAssetWriter
-  movieTimeScale 

Instance Property

# movieTimeScale

The time scale of the movie.

iOS 4.3+iPadOS 4.3+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var movieTimeScale: CMTimeScale { get set }
```

## Discussion

The default value is `0`, which indicates that the asset writer chooses an appropriate value, if applicable.

You can’t set this property value after writing starts.

## See Also

### Configuring Fragment Output

var movieFragmentInterval: CMTime

The interval at which to write movie fragments.

var initialMovieFragmentInterval: CMTime

The interval at which to write the initial movie fragment.

var initialMovieFragmentSequenceNumber: Int

The sequence number of the initial movie fragment.

var producesCombinableFragments: Bool

A Boolean value that indicates whether the asset writer outputs movie fragments suitable for combining with others.

var overallDurationHint: CMTime

A hint of the final duration of the output file.

