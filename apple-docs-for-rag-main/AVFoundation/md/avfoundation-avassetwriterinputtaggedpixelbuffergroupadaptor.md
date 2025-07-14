

- AVFoundation
-  AVAssetWriterInputTaggedPixelBufferGroupAdaptor 

Class

# AVAssetWriterInputTaggedPixelBufferGroupAdaptor

An object that appends tagged buffer groups to an asset writer input.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
class AVAssetWriterInputTaggedPixelBufferGroupAdaptor
```

## Overview

This class provides a CVPixelBufferPool to use for allocating the pixel buffers of tagged buffer groups to write to the output file. Using the provided pixel buffer pool for buffer allocation is typically more efficient than appending pixel buffers allocated using a separate pool.

## Topics

### Creating an adaptor

init(assetWriterInput: AVAssetWriterInput, sourcePixelBufferAttributes: [String : Any]?)

Creates an object that appends tagged buffer groups to an asset writer input.

### Configuring the buffer pool

var sourcePixelBufferAttributes: [String : Any]?

The attributes of buffers that the adaptor’s pixel buffer pool vends.

var pixelBufferPool: CVPixelBufferPool?

A pixel buffer pool that vends and efficiently recycles the pixel buffers of tagged buffer groups.

### Appending pixel buffers

func appendTaggedBuffers([CMTaggedBuffer], withPresentationTime: CMTime) -> Bool

Appends a tagged buffer group to the adaptor.

func appendTaggedPixelBufferGroup(__CMTaggedBufferGroup, withPresentationTime: CMTime) -> Bool

Appends a tagged buffer group to the adaptor.

### Accessing the writer input

var assetWriterInput: AVAssetWriterInput

The asset writer input to which the adaptor appends tagged buffer groups.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Media writing

Writing Fragmented MPEG-4 Files for HTTP Live Streaming

Create an HTTP Live Streaming presentation by turning a movie file into a sequence of fragmented MPEG-4 files.

Converting side-by-side 3D video to multiview HEVC and spatial video

Create video content for visionOS by converting an existing 3D HEVC file to a multiview HEVC format, optionally adding spatial metadata to create a spatial video.

Creating spatial photos and videos with spatial metadata

Add spatial metadata to stereo photos and videos to create spatial media for viewing on Apple Vision Pro.

Tagging Media with Video Color Information

Inspect and set video color space information when writing and transcoding media.

Evaluating an App’s Video Color

Check color reproduction for a video in your app by using test patterns, video test equipment, and light-measurement instruments.

class AVOutputSettingsAssistant

An object that builds audio and video output settings dictionaries.

class AVAssetWriter

An object that writes media data to a container file.

class AVAssetWriterInput

An object that appends media samples to a track in an asset writer’s output file.

class AVAssetWriterInputPixelBufferAdaptor

An object that appends video samples to an asset writer input.

class AVAssetWriterInputMetadataAdaptor

An object that appends timed metadata groups to an asset writer input.

class AVAssetWriterInputGroup

A group of inputs with tracks that are mutually exclusive to each other for playback or processing.

