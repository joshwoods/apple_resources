

- AVFoundation
- AVAssetWriter
-  overallDurationHint 

Instance Property

# overallDurationHint

A hint of the final duration of the output file.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var overallDurationHint: CMTime { get set }
```

## Discussion

The default value of invalid indicates that the asset writer doesn’t write an overall duration hint to the file. The asset writer ignores this value if it doesn’t write movie fragments.

You can’t set this property after writing starts.

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

var movieTimeScale: CMTimeScale

The time scale of the movie.

