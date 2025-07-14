

- AVFoundation
-  AVAssetWriterInputGroup 

Class

# AVAssetWriterInputGroup

A group of inputs with tracks that are mutually exclusive to each other for playback or processing.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
class AVAssetWriterInputGroup
```

## Overview

Assets may contain multiple tracks of media that are mutually exclusive to each other when you play or process them. For example, an asset may contain multiple audio tracks for different spoken languages, but only one of them should play at a time. You use an input group to mark a collection of tracks as mutually exclusive to each other in the file the asset writer outputs.

Note

After associating several tracks by calling addTrackAssociation(withTrackOf:type:), you can examine the media selection options an asset writer outputs before it writes the file.

## Topics

### Creating an Input Group

init(inputs: [AVAssetWriterInput], defaultInput: AVAssetWriterInput?)

Creates a group for the asset writer inputs.

### Accessing the Inputs

var inputs: [AVAssetWriterInput]

The inputs with tracks that are mutually exclusive to each other for playback or processing.

var defaultInput: AVAssetWriterInput?

The default input for the group.

## Relationships

### Inherits From

- AVMediaSelectionGroup

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
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

class AVAssetWriterInputMetadataAdaptor

An object that appends timed metadata groups to an asset writer input.

