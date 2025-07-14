

- AVFoundation
- AVMutableMovieTrack
-  preferredMediaChunkDuration 

Instance Property

# preferredMediaChunkDuration

The maximum duration to use for each chunk of sample data written to the file for file types that support media chunk duration.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
var preferredMediaChunkDuration: CMTime { get set }
```

## Discussion

The total duration of the samples in a chunk can be no greater than the preferred chunk duration, or the duration of a single sample if the single sample’s duration is greater than the preferred chunk duration. The default media chunk duration is `1.0` second. Setting a negative or non-numeric value for the chunk duration will cause an error.

## See Also

### Accessing Media Chunks

var preferredMediaChunkAlignment: Int

The boundary for media chunk alignment for file types that support media chunk alignment.

var preferredMediaChunkSize: Int

The maximum size to use for each chunk of sample data written to the file for file types that support media chunk duration.

