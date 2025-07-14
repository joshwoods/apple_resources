

- AVFoundation
- AVAssetWriterInput
-  preferredMediaChunkAlignment 

Instance Property

# preferredMediaChunkAlignment

The boundary, in bytes, for aligning media chunks.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var preferredMediaChunkAlignment: Int { get set }
```

## Discussion

This property supports file types that support media chunk alignment, such as QuickTime Movie files. The default value is `0`, which means that the input chooses an appropriate default value. A value of `1` indicates not to use padding to achieve a particular chunk alignment. It’s an error to set a negative value for chunk alignment.

You can’t set this value after writing starts.

## See Also

### Configuring Media Data Layout

var preferredMediaChunkDuration: CMTime

The duration to use for each chunk of sample data in the output file.

var sampleReferenceBaseURL: URL?

The base URL sample references are relative to.

var mediaDataLocation: AVAssetWriterInput.MediaDataLocation

Specifies how the input lays out and interleaves media data.

struct MediaDataLocation

A structure that indicates how to lay out and interleave media data.

