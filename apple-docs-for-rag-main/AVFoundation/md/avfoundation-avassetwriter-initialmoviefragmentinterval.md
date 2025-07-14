

- AVFoundation
- AVAssetWriter
-  initialMovieFragmentInterval 

Instance Property

# initialMovieFragmentInterval

The interval at which to write the initial movie fragment.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
var initialMovieFragmentInterval: CMTime { get set }
```

## Discussion

When using fragment writing, you can set this property value to indicate the interval at which to write the initial fragment.

The default value is invalid, which indicates to use the interval set in the movieFragmentInterval property. The movieFragmentInterval property is typically set to 10 seconds, so if an error occurs before writing the first fragment, the movie file won’t be playable. To avoid this case, your app may want to set a shorter interval, such as 1 second, to write the initial fragment, and then use a 10 second interval for subsequent fragments.

You can’t set this property after writing starts.

## See Also

### Configuring Fragment Output

var movieFragmentInterval: CMTime

The interval at which to write movie fragments.

var initialMovieFragmentSequenceNumber: Int

The sequence number of the initial movie fragment.

var producesCombinableFragments: Bool

A Boolean value that indicates whether the asset writer outputs movie fragments suitable for combining with others.

var overallDurationHint: CMTime

A hint of the final duration of the output file.

var movieTimeScale: CMTimeScale

The time scale of the movie.

