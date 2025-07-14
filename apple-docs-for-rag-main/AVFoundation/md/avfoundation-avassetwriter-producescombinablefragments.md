

- AVFoundation
- AVAssetWriter
-  producesCombinableFragments 

Instance Property

# producesCombinableFragments

A Boolean value that indicates whether the asset writer outputs movie fragments suitable for combining with others.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var producesCombinableFragments: Bool { get set }
```

## Discussion

The default value is false. Set the value to true when you use multiple asset writers to produce distinct streams that complement each other, such as HLS encodings or bit rate variants.

You can’t set this property after writing starts.

## See Also

### Configuring Fragment Output

var movieFragmentInterval: CMTime

The interval at which to write movie fragments.

var initialMovieFragmentInterval: CMTime

The interval at which to write the initial movie fragment.

var initialMovieFragmentSequenceNumber: Int

The sequence number of the initial movie fragment.

var overallDurationHint: CMTime

A hint of the final duration of the output file.

var movieTimeScale: CMTimeScale

The time scale of the movie.

