

- AVFoundation
- AVMutableVideoComposition
-  videoComposition(withPropertiesOf:completionHandler:) 

Type Method

# videoComposition(withPropertiesOf:completionHandler:)

Returns a new video composition that’s configured to present the video tracks of the specified asset.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
class func videoComposition(
    withPropertiesOf asset: AVAsset,
    completionHandler: @escaping (AVMutableVideoComposition?, (any Error)?) -> Void
)
```

``` source
class func videoComposition(withPropertiesOf asset: AVAsset) async throws -> AVMutableVideoComposition
```

## Parameters 

`asset`  

An asset to create a video composition for.

`completionHandler`  

A callback the system invokes with the created video composition, or an error if a failure occurs.

## Discussion

This method creates the video composition object and configures it with the values and instructions suitable for presenting the video tracks of the specified asset. The returned object contains instructions that respect the spatial properties and time ranges of the specified asset’s video tracks. It also configures the object properties in the following way:

- The value of the frameDuration property is short enough to accommodate the greatest nominal frame rate value among the asset’s video tracks, as indicated by the nominalFrameRate property of each track. If all its tracks have a nominal frame rate of `0`, it uses a frame rate of 30 frames per second, with the frame duration set accordingly.

- The value of the renderSize property depends on whether the asset is an AVComposition object. For an AVComposition, the render size is the composition’s naturalSize value, and for other assets, its a size large enough to encompass all of its video tracks.

- The value of the renderScale property is `1.0`.

- The value of the animationTool property is `nil`.

Note

If you specify an asset that doesn’t contain video tracks, this method returns a video composition with no instructions.

## See Also

### Creating a Video Composition

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

