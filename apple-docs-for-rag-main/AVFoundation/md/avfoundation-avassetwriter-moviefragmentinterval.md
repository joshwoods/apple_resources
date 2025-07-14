

- AVFoundation
- AVAssetWriter
-  movieFragmentInterval 

Instance Property

# movieFragmentInterval

The interval at which to write movie fragments.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var movieFragmentInterval: CMTime { get set }
```

## Discussion

Some container formats, such as QuickTime movies, support writing movies in fragments. Using this feature enables you to open and play a partially written movie in the event that an unexpected error or interruption occurs.

An asset writer disables this feature by default and sets this value to invalid. To enable fragment writing, set a valid CMTime value. For best performance when writing to external storage devices, set the movie fragment interval to 10 seconds or greater.

You can’t set this value after writing starts.

## See Also

### Configuring Fragment Output

var initialMovieFragmentInterval: CMTime

The interval at which to write the initial movie fragment.

var initialMovieFragmentSequenceNumber: Int

The sequence number of the initial movie fragment.

var producesCombinableFragments: Bool

A Boolean value that indicates whether the asset writer outputs movie fragments suitable for combining with others.

var overallDurationHint: CMTime

A hint of the final duration of the output file.

var movieTimeScale: CMTimeScale

The time scale of the movie.

