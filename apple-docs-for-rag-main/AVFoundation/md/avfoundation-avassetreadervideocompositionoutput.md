

- AVFoundation
-  AVAssetReaderVideoCompositionOutput 

Class

# AVAssetReaderVideoCompositionOutput

An object that reads composited video frames from one or more tracks of an asset.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
class AVAssetReaderVideoCompositionOutput
```

## Topics

### Creating a Video Composition Output

init(videoTracks: [AVAssetTrack], videoSettings: [String : Any]?)

Creates an object that reads composited video frames from the specified video tracks.

### Configuring Video Settings

var videoComposition: AVVideoComposition?

The video composition to use for the output.

var customVideoCompositor: (any AVVideoCompositing)?

A custom video compositor for the output.

### Inspecting an Output

var videoTracks: [AVAssetTrack]

The tracks from which the output reads the composited video.

var videoSettings: [String : Any]?

The video settings that the output uses.

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

class AVAssetReaderSampleReferenceOutput

An object that reads sample references from an asset track.

class AVAssetReaderOutputMetadataAdaptor

An object that creates timed metadata group objects for an asset track.

