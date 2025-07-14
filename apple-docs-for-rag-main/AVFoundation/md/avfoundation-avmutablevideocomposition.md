

- AVFoundation
-  AVMutableVideoComposition 

Class

# AVMutableVideoComposition

A mutable video composition subclass.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
class AVMutableVideoComposition
```

## Overview

If you use the built-in video compositor, the instructions a video composition contain can specify a spatial transformation, an opacity value, and a cropping rectangle for each video source. This values can vary over time by applying linear ramping functions.

You can create a custom video compositor by implementing the AVVideoCompositing protocol. The system provides the custom video compositor with pixel buffers for each of its video sources during playback, and can perform arbitrary graphical operations on them to produce visual output.

## Topics

### Creating a Video Composition

class func videoComposition(withPropertiesOf: AVAsset, completionHandler: (AVMutableVideoComposition?, (any Error)?) -> Void)

Returns a new video composition that’s configured to present the video tracks of the specified asset.

class func videoComposition(withPropertiesOf: AVAsset, prototypeInstruction: AVVideoCompositionInstruction, completionHandler: (AVMutableVideoComposition?, (any Error)?) -> Void)

Returns a new mutable video composition with the specified asset properties and a prototype video composition instruction.

class func videoComposition(with: AVAsset, applyingCIFiltersWithHandler: (AVAsynchronousCIImageFilteringRequest) -> Void, completionHandler: (AVMutableVideoComposition?, (any Error)?) -> Void)

Returns a new video composition that’s configured to apply Core Image filters to each video frame of the specified asset.

init(propertiesOf: AVAsset)

Creates a mutable video composition with the specified asset properties.

Deprecated

init(propertiesOf: AVAsset, prototypeInstruction: AVVideoCompositionInstruction)

Creates a mutable video composition with the specified asset properties and a prototype video composition instruction.

Deprecated

init(asset: AVAsset, applyingCIFiltersWithHandler: (AVAsynchronousCIImageFilteringRequest) -> Void)

Creates a mutable video composition configured to apply Core Image filters to each video frame of the specified asset.

Deprecated

### Configuring Video Composition Properties

var frameDuration: CMTime

A time interval for which the video composition should render composed video frames.

var renderSize: CGSize

The size at which the video composition should render.

var renderScale: Float

The scale at which the video composition should render.

var animationTool: AVVideoCompositionCoreAnimationTool?

A video composition tool to use with Core Animation in offline rendering.

### Specifying composition instructions

var instructions: [any AVVideoCompositionInstructionProtocol]

The video composition instructions.

protocol AVVideoCompositionInstructionProtocol

A protocol that defines the interface for a video composition instruction.

### Configuring HDR Metadata

var perFrameHDRDisplayMetadataPolicy: AVVideoComposition.PerFrameHDRDisplayMetadataPolicy

Configures the policy for display of HDR display metadata on the rendered frame.

struct PerFrameHDRDisplayMetadataPolicy

A type that defines the policy for handling of per frame HDR metadata.

### Configuring Color

var colorPrimaries: String?

The color primaries used for video composition.

var colorTransferFunction: String?

The transfer function used for video composition.

var colorYCbCrMatrix: String?

The YCbCr matrix used for video composition.

### Identifying Source Tracks

var sourceTrackIDForFrameTiming: CMPersistentTrackID

An identifier of the source track from which the video composition derives frame timing.

var sourceSampleDataTrackIDs: [CMPersistentTrackID]

The identifiers of source sample data tracks in the composition that the object requires to compose frames.

### Specifying a custom compositor

var customVideoCompositorClass: (any AVVideoCompositing.Type)?

The custom compositor class to use.

## Relationships

### Inherits From

- AVVideoComposition

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

class AVVideoComposition

An object that describes how to compose video frames at particular points in time.

class AVVideoCompositionInstruction

An operation that a compositor performs.

class AVMutableVideoCompositionInstruction

A mutable video composition instruction subclass.

class AVVideoCompositionLayerInstruction

An object used to modify the transform, cropping, and opacity ramps applied to a given track in a composition.

class AVMutableVideoCompositionLayerInstruction

An object used to modify the transform, cropping, and opacity ramps applied to a given track in a mutable composition.

