

- AVFoundation
- AVAssetWriterInput
-  mediaDataLocation 

Instance Property

# mediaDataLocation

Specifies how the input lays out and interleaves media data.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var mediaDataLocation: AVAssetWriterInput.MediaDataLocation { get set }
```

## Discussion

Use this property to optimize tracks that contain a small amount of data that you need all at once, such as chapter tracks. Setting the value to beforeMainMediaDataNotInterleaved causes the asset writer to try to write the media data for this track before interleaved inputs. For file types that support preloading media data, such as QuickTime files, setting this value also writes an indicator to the file to preload its media data.

Set the value to interleavedWithMainMediaData for tracks whose media data you need only as it approaches its presentation time, or when multiple inputs exist that supply media data that plays concurrently.

You can’t set this value after writing starts.

## See Also

### Configuring Media Data Layout

var preferredMediaChunkAlignment: Int

The boundary, in bytes, for aligning media chunks.

var preferredMediaChunkDuration: CMTime

The duration to use for each chunk of sample data in the output file.

var sampleReferenceBaseURL: URL?

The base URL sample references are relative to.

struct MediaDataLocation

A structure that indicates how to lay out and interleave media data.

