

- AVFoundation
-  AVAssetReaderOutput 

Class

# AVAssetReaderOutput

An abstract class that defines the interface to read media samples from an asset reader.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
class AVAssetReaderOutput
```

## Mentioned in 

Tagging Media with Video Color Information

## Overview

You add concrete output instances, such as AVAssetReaderTrackOutput or AVAssetReaderVideoCompositionOutput, to an asset reader to perform specific tasks.

Important

If you don’t require modifying sample data in-place, set the value of the alwaysCopiesSampleData property to false to prevent the output from making unnecessary copies.

## Topics

### Configuring Reading

var alwaysCopiesSampleData: Bool

A Boolean value that indicates whether the output vends copied sample data.

var supportsRandomAccess: Bool

A Boolean value that indicates whether the output supports reconfiguring the time ranges it reads.

func reset(forReadingTimeRanges: [NSValue])

Restarts reading with a new set of time ranges.

func markConfigurationAsFinal()

Tells the output that it’s finished reconfiguring time ranges, and allows the asset reader to advance to a completed state.

### Copying Sample Buffers

func copyNextSampleBuffer() -> CMSampleBuffer?

Copies the next sample buffer from the output.

### Inspecting the Media Type

var mediaType: AVMediaType

The media type of samples that the output reads.

## Relationships

### Inherits From

- NSObject

### Inherited By

- AVAssetReaderAudioMixOutput
- AVAssetReaderSampleReferenceOutput
- AVAssetReaderTrackOutput
- AVAssetReaderVideoCompositionOutput

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Media reading

Reading multiview 3D video files

Render single images for the left eye and right eye from a multiview High Efficiency Video Coding format file by reading individual video frames.

class AVAssetReader

An object that reads media data from an asset.

class AVAssetReaderTrackOutput

An object that reads media data from a single track of an asset.

class AVAssetReaderAudioMixOutput

An object that reads audio samples that result from mixing audio from one or more tracks.

class AVAssetReaderVideoCompositionOutput

An object that reads composited video frames from one or more tracks of an asset.

class AVAssetReaderSampleReferenceOutput

An object that reads sample references from an asset track.

class AVAssetReaderOutputMetadataAdaptor

An object that creates timed metadata group objects for an asset track.

