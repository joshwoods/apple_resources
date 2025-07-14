

- AVFoundation
- AVAssetWriterInput
-  AVAssetWriterInput.MediaDataLocation 

Structure

# AVAssetWriterInput.MediaDataLocation

A structure that indicates how to lay out and interleave media data.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
struct MediaDataLocation
```

## Topics

### Media Data Locations

static let interleavedWithMainMediaData: AVAssetWriterInput.MediaDataLocation

A value that indicates to interleave the input’s media data with other media data.

static let beforeMainMediaDataNotInterleaved: AVAssetWriterInput.MediaDataLocation

A value that indicates to use noninterleaved data, and write it before interleaved data.

### Initializers

init(rawValue: String)

Creates a location with a string value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring Media Data Layout

var preferredMediaChunkAlignment: Int

The boundary, in bytes, for aligning media chunks.

var preferredMediaChunkDuration: CMTime

The duration to use for each chunk of sample data in the output file.

var sampleReferenceBaseURL: URL?

The base URL sample references are relative to.

var mediaDataLocation: AVAssetWriterInput.MediaDataLocation

Specifies how the input lays out and interleaves media data.

