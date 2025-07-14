

- AVFoundation
-  AVVideoComposition 

Class

# AVVideoComposition

An object that describes how to compose video frames at particular points in time.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
class AVVideoComposition
```

## Overview

If you use the built-in video compositor, the instructions a video composition contain can specify a spatial transformation, an opacity value, and a cropping rectangle for each video source. This values can vary over time by applying linear ramping functions.

You can create a custom video compositor by implementing the AVVideoCompositing protocol. The system provides the custom video compositor with pixel buffers for each of its video sources during playback, and can perform arbitrary graphical operations on them to produce visual output.

## Topics

### Creating a Video Composition

class func videoComposition(withPropertiesOf: AVAsset, completionHandler: (AVVideoComposition?, (any Error)?) -> Void)

Returns a new video composition that’s configured to present the video tracks of the specified asset.

class func videoComposition(with: AVAsset, applyingCIFiltersWithHandler: (AVAsynchronousCIImageFilteringRequest) -> Void, completionHandler: (AVVideoComposition?, (any Error)?) -> Void)

Returns a new video composition that’s configured to apply Core Image filters to each video frame of the specified asset.

class AVAsynchronousCIImageFilteringRequest

An object that supports using Core Image filters to process an individual video frame in a video composition.

init(propertiesOf: AVAsset)

Creates a video composition object configured to present the video tracks of the specified asset.

Deprecated

init(asset: AVAsset, applyingCIFiltersWithHandler: (AVAsynchronousCIImageFilteringRequest) -> Void)

Creates a video composition configured to apply Core Image filters to each video frame of the specified asset.

Deprecated

### Inspecting the Video Composition

var renderSize: CGSize

The size at which the video composition should render.

var renderScale: Float

The scale at which the video composition should render.

var frameDuration: CMTime

A time interval for which the video composition should render composed video frames.

var animationTool: AVVideoCompositionCoreAnimationTool?

A video composition tool to use with Core Animation in offline rendering.

var colorPrimaries: String?

The color primaries used for video composition.

var colorTransferFunction: String?

The transfer function used for video composition.

var colorYCbCrMatrix: String?

The YCbCr matrix used for video composition.

var customVideoCompositorClass: (any AVVideoCompositing.Type)?

A custom compositor class to use.

### Validating the Time Range

func isValid(for: [AVAssetTrack], assetDuration: CMTime, timeRange: CMTimeRange, validationDelegate: (any AVVideoCompositionValidationHandling)?) -> Bool

Indicates whether the time ranges of the composition’s instructions conform to validation requirements.

protocol AVVideoCompositionValidationHandling

Methods you can implement to indicate whether validation of a video composition should continue after specific errors are found.

func determineValidity(for: AVAsset?, timeRange: CMTimeRange, validationDelegate: (any AVVideoCompositionValidationHandling)?, completionHandler: (Bool, (any Error)?) -> Void)

Determines whether the time ranges of the composition’s instructions conform to validation requirements.

Deprecated

func isValid(for: AVAsset?, timeRange: CMTimeRange, validationDelegate: (any AVVideoCompositionValidationHandling)?) -> Bool

Indicates whether the time ranges of the composition’s instructions conform to validation requirements.

Deprecated

### Reading Instructions

var instructions: [any AVVideoCompositionInstructionProtocol]

The video composition instructions.

protocol AVVideoCompositionInstructionProtocol

A protocol that defines the interface for a video composition instruction.

### Identifying Source Tracks

var sourceTrackIDForFrameTiming: CMPersistentTrackID

An identifier of the source track from which the video composition derives frame timing.

var sourceSampleDataTrackIDs: [CMPersistentTrackID]

The identifiers of source sample data tracks in the composition that the object requires to compose frames.

### Configuring HDR Metadata

var perFrameHDRDisplayMetadataPolicy: AVVideoComposition.PerFrameHDRDisplayMetadataPolicy

The policy for display of HDR display metadata on the rendered frame.

struct PerFrameHDRDisplayMetadataPolicy

A type that defines the policy for handling of per frame HDR metadata.

## Relationships

### Inherits From

- NSObject

### Inherited By

- AVMutableVideoComposition

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSMutableCopying
- NSObjectProtocol

## See Also

### Built-in video compositing

Editing and Playing HDR Video

Support high-dynamic-range (HDR) video content in your app by using the HDR editing and playback capabilities of AVFoundation.

Debugging AVFoundation audio mixes, compositions, and video compositions

Resolve common problems when creating compositions, video compositions, and audio mixes.

class AVMutableVideoComposition

A mutable video composition subclass.

class AVVideoCompositionInstruction

An operation that a compositor performs.

class AVMutableVideoCompositionInstruction

A mutable video composition instruction subclass.

class AVVideoCompositionLayerInstruction

An object used to modify the transform, cropping, and opacity ramps applied to a given track in a composition.

class AVMutableVideoCompositionLayerInstruction

An object used to modify the transform, cropping, and opacity ramps applied to a given track in a mutable composition.

