

- AVFoundation
-  AVAssetWriterInputPixelBufferAdaptor 

Class

# AVAssetWriterInputPixelBufferAdaptor

An object that appends video samples to an asset writer input.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
class AVAssetWriterInputPixelBufferAdaptor
```

## Overview

A pixel buffer adaptor provides a pixel buffer pool that you use to allocate pixel buffers to the output file. Using the provided pool for buffer allocation is typically more efficient than managing your own pool.

## Topics

### Creating an Adaptor

init(assetWriterInput: AVAssetWriterInput, sourcePixelBufferAttributes: [String : Any]?)

Creates a new pixel buffer adaptor to receive pixel buffers for writing to the output file.

### Appending Pixel Buffers

func append(CVPixelBuffer, withPresentationTime: CMTime) -> Bool

Appends a pixel buffer to the adaptor.

### Accessing the Pool

var pixelBufferPool: CVPixelBufferPool?

A pool of pixel buffers to append to the adaptor’s input.

var sourcePixelBufferAttributes: [String : Any]?

The attributes of the pixel buffers that the pool contains.

### Inspecting a Pixel Buffer Adaptor

var assetWriterInput: AVAssetWriterInput

The asset writer input to which the adaptor appends pixel buffers.

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

class AVAssetWriterInputTaggedPixelBufferGroupAdaptor

An object that appends tagged buffer groups to an asset writer input.

class AVAssetWriterInputMetadataAdaptor

An object that appends timed metadata groups to an asset writer input.

class AVAssetWriterInputGroup

A group of inputs with tracks that are mutually exclusive to each other for playback or processing.

