

- AVFoundation
-  AVAssetReaderSampleReferenceOutput 

Class

# AVAssetReaderSampleReferenceOutput

An object that reads sample references from an asset track.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
class AVAssetReaderSampleReferenceOutput
```

## Overview

Apps can extract information about the location of samples in a track — the file URL and offset — by adding an instance of this class to an asset reader. Read the kCMSampleBufferAttachmentKey_SampleReferenceURL and kCMSampleBufferAttachmentKey_SampleReferenceByteOffset attachments on the extracted sample buffers to get the location of the sample data.

You can also append sample buffers that you extract using this class to an AVAssetWriterInput instance to create movie tracks that aren’t self-contained and reference data in the original file instead. To write tracks that aren’t self-contained, use instances of AVAssetWriter that you configure to write files of type mov.

Because this output doesn’t return sample data, it ignores the value of the alwaysCopiesSampleData property.

## Topics

### Creating a Sample Reference Output

init(track: AVAssetTrack)

Creates an object that supplies sample references.

### Inspecting the Track

var track: AVAssetTrack

The track from which the output reads sample references.

## Relationships

### Inherits From

- AVAssetReaderOutput

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

class AVAssetReaderOutput

An abstract class that defines the interface to read media samples from an asset reader.

class AVAssetReaderTrackOutput

An object that reads media data from a single track of an asset.

class AVAssetReaderAudioMixOutput

An object that reads audio samples that result from mixing audio from one or more tracks.

class AVAssetReaderVideoCompositionOutput

An object that reads composited video frames from one or more tracks of an asset.

class AVAssetReaderOutputMetadataAdaptor

An object that creates timed metadata group objects for an asset track.

