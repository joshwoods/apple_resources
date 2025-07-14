

- AVFoundation
-  AVAssetReaderTrackOutput 

Class

# AVAssetReaderTrackOutput

An object that reads media data from a single track of an asset.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
class AVAssetReaderTrackOutput
```

## Overview

Read the media data of an asset track by adding a track output to an asset reader. You can read the media samples in their stored format, or you can convert them to an alternative format.

A track output produces uncompressed output. For audio output settings, this means that AVFormatIDKey must be kAudioFormatLinearPCM. For video output settings, this means that the dictionary must contain values for uncompressed video output, as defined in `Video Settings`. A track output doesn’t support the AVSampleRateConverterAudioQualityKey audio setting key or the following video settings keys: AVVideoCleanApertureKey, AVVideoPixelAspectRatioKey, and AVVideoScalingModeKey.

When constructing video output settings, the choice of pixel format affects the performance and quality of the decompression. For optimal performance when decompressing video, the requested pixel format should be one that the decoder supports natively to avoid unnecessary conversions. Below are some recommendations:

- For H.264, use kCVPixelFormatType_420YpCbCr8BiPlanarVideoRange or kCVPixelFormatType_420YpCbCr8BiPlanarFullRange when you know the video is full range.

- In iOS, use kCVPixelFormatType_420YpCbCr8BiPlanarFullRange for JPEG output.

- In macOS, kCVPixelFormatType_422YpCbCr8 is the preferred pixel format for video and generally provides the best performance when decoding. If you need to work in the RGB domain, use kCVPixelFormatType_32BGRA in iOS, and kCVPixelFormatType_32ARGB in macOS.

- ProRes-encoded media can contain up to 12 bits per channel. For ProRes-encoded sources that you wish to preserve more than 8 bits per channel during decompression, use one of the following pixel formats: kCVPixelFormatType_4444AYpCbCr16, kCVPixelFormatType_422YpCbCr16, kCVPixelFormatType_422YpCbCr10, or kCVPixelFormatType_64ARGB. AVAssetReader doesn’t support scaling with any of these high-bit-depth pixel formats. If you use the above pixel formats, don’t specify kCVPixelBufferWidthKey or kCVPixelBufferHeightKey in the outputSettings dictionary. Only ProRes encoders support these pixel formats.

- ProRes 4444-encoded media can contain a mathematically lossless alpha channel. To preserve the alpha channel during decompression, use a pixel format with an alpha component such as kCVPixelFormatType_4444AYpCbCr16 or kCVPixelFormatType_64ARGB. To test whether your source contains an alpha channel, check that the track’s format description has a kCMFormatDescriptionExtension_Depth key with a value of `32`.

## Topics

### Creating a Track Output

init(track: AVAssetTrack, outputSettings: [String : Any]?)

Creates an object that reads media data from an asset track.

Video settings

Configure video processing settings using standard key and value constants.

### Configuring Audio Settings

var audioTimePitchAlgorithm: AVAudioTimePitchAlgorithm

The processing algorithm to use for scaled audio edits.

### Inspecting an Output

var outputSettings: [String : Any]?

The output settings for this track output.

var track: AVAssetTrack

The track from which the output reads sample buffers.

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

class AVAssetReaderAudioMixOutput

An object that reads audio samples that result from mixing audio from one or more tracks.

class AVAssetReaderVideoCompositionOutput

An object that reads composited video frames from one or more tracks of an asset.

class AVAssetReaderSampleReferenceOutput

An object that reads sample references from an asset track.

class AVAssetReaderOutputMetadataAdaptor

An object that creates timed metadata group objects for an asset track.

