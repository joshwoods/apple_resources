

- AVFoundation
-  AVAssetReaderOutputMetadataAdaptor 

Class

# AVAssetReaderOutputMetadataAdaptor

An object that creates timed metadata group objects for an asset track.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
class AVAssetReaderOutputMetadataAdaptor
```

## Topics

### Creating a Metadata Adaptor

init(assetReaderTrackOutput: AVAssetReaderTrackOutput)

Creates an object that reads timed metadata groups from an asset reader output.

### Retrieving Timed Metadata Groups

func nextTimedMetadataGroup() -> AVTimedMetadataGroup?

Returns the next timed metadata group for the asset reader output.

### Inspecting the Track Output

var assetReaderTrackOutput: AVAssetReaderTrackOutput

The asset reader track output that provides the timed metadata groups.

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

class AVAssetReaderSampleReferenceOutput

An object that reads sample references from an asset track.

