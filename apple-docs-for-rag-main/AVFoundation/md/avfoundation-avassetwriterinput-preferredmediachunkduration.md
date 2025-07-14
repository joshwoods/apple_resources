

- AVFoundation
- AVAssetWriterInput
-  preferredMediaChunkDuration 

Instance Property

# preferredMediaChunkDuration

The duration to use for each chunk of sample data in the output file.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var preferredMediaChunkDuration: CMTime { get set }
```

## Discussion

This property supports file types that support media chunk alignment, such as QuickTime Movie files. Chunk duration can influence the granularity of the I/O the system performs when reading a media file; for example, during playback. A larger chunk duration can result in fewer reads from disk, at the potential expense of a higher memory footprint.

A chunk contains one or more samples. The total duration of the samples in a chunk is no greater than the preferred chunk duration, or the duration of a single sample if the sample’s duration is greater than this preferred chunk duration.

The default value is invalid, which means that the input chooses an appropriate default value. It’s an error to set a chunk duration that’s negative or nonnumeric.

You can’t set this value after writing starts.

## See Also

### Configuring Media Data Layout

var preferredMediaChunkAlignment: Int

The boundary, in bytes, for aligning media chunks.

var sampleReferenceBaseURL: URL?

The base URL sample references are relative to.

var mediaDataLocation: AVAssetWriterInput.MediaDataLocation

Specifies how the input lays out and interleaves media data.

struct MediaDataLocation

A structure that indicates how to lay out and interleave media data.

