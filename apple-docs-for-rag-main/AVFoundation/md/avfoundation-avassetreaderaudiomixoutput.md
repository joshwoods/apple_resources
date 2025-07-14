

- AVFoundation
-  AVAssetReaderAudioMixOutput 

Class

# AVAssetReaderAudioMixOutput

An object that reads audio samples that result from mixing audio from one or more tracks.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
class AVAssetReaderAudioMixOutput
```

## Overview

Read audio data that you mix from one or more asset tracks by adding an audio mix output to an asset reader. You can read the samples in their stored format or you can convert them to an alternative format.

## Topics

### Creating an Audio Mix Output

init(audioTracks: [AVAssetTrack], audioSettings: [String : Any]?)

Creates an object that reads mixed audio from the specified audio tracks.

### Configuring Audio Settings

var audioMix: AVAudioMix?

The audio mix to use with this output.

var audioTimePitchAlgorithm: AVAudioTimePitchAlgorithm

The processing algorithm to use for scaled audio edits.

### Inspecting an Output

var audioTracks: [AVAssetTrack]

The tracks from which the output reads audio.

var audioSettings: [String : Any]?

The audio settings that the output uses.

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

class AVAssetReaderVideoCompositionOutput

An object that reads composited video frames from one or more tracks of an asset.

class AVAssetReaderSampleReferenceOutput

An object that reads sample references from an asset track.

class AVAssetReaderOutputMetadataAdaptor

An object that creates timed metadata group objects for an asset track.

