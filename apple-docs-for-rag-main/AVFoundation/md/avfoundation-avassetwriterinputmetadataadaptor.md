

- AVFoundation
-  AVAssetWriterInputMetadataAdaptor 

Class

# AVAssetWriterInputMetadataAdaptor

An object that appends timed metadata groups to an asset writer input.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
class AVAssetWriterInputMetadataAdaptor
```

## Overview

Use a metadata adaptor to append track-level metadata, packaged as instances of AVTimedMetadataGroup, to an asset writer input.

## Topics

### Creating an Input Metadata Adaptor

init(assetWriterInput: AVAssetWriterInput)

Creates a metadata group adaptor to append timed metadata groups to write to an output file.

### Appending Timed Metadata

func append(AVTimedMetadataGroup) -> Bool

Appends a timed metadata group to the adaptor.

### Accessing the Input

var assetWriterInput: AVAssetWriterInput

The input for the metadata adaptor.

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

class AVAssetWriterInputTaggedPixelBufferGroupAdaptor

An object that appends tagged buffer groups to an asset writer input.

class AVAssetWriterInputGroup

A group of inputs with tracks that are mutually exclusive to each other for playback or processing.

