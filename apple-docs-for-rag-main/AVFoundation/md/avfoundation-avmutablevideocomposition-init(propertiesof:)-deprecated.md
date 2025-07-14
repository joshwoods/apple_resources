

- AVFoundation
- AVMutableVideoComposition
-  init(propertiesOf:) Deprecated

Initializer

# init(propertiesOf:)

Creates a mutable video composition with the specified asset properties.

iOS 6.0–18.0DeprecatediPadOS 6.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.9–15.0DeprecatedtvOS 9.0–18.0Deprecated

``` source
init(propertiesOf asset: AVAsset)
```

Deprecated

Use videoCompositionWithPropertiesOfAsset:completionHandler: instead

## Parameters 

`asset`  

An instance of AVAsset. Ensure that the duration and tracks properties of the asset are already loaded before invoking this method.

## Discussion

The returned `AVMutableVideoComposition` has instructions that respect the spatial properties and time ranges of the specified asset’s video tracks.

It also has the following values for its properties:

- A value for frameDuration short enough to accommodate the greatest nominalFrameRate among the asset’s video tracks. If the nominalFrameRate of all of the asset’s video tracks is 0, a default frame rate of 30fps is used.

- If the specified asset is an instance of AVComposition, the renderSize is set to the naturalSize of the AVComposition; otherwise the renderSize will be set to a value that encompasses all of the asset’s video tracks.

- A renderScale of 1.0.

- The animationTool property set to `nil`.

## See Also

### Creating a Video Composition

class func videoComposition(withPropertiesOf: AVAsset, completionHandler: (AVMutableVideoComposition?, (any Error)?) -> Void)

Returns a new video composition that’s configured to present the video tracks of the specified asset.

class func videoComposition(withPropertiesOf: AVAsset, prototypeInstruction: AVVideoCompositionInstruction, completionHandler: (AVMutableVideoComposition?, (any Error)?) -> Void)

Returns a new mutable video composition with the specified asset properties and a prototype video composition instruction.

class func videoComposition(with: AVAsset, applyingCIFiltersWithHandler: (AVAsynchronousCIImageFilteringRequest) -> Void, completionHandler: (AVMutableVideoComposition?, (any Error)?) -> Void)

Returns a new video composition that’s configured to apply Core Image filters to each video frame of the specified asset.

init(propertiesOf: AVAsset, prototypeInstruction: AVVideoCompositionInstruction)

Creates a mutable video composition with the specified asset properties and a prototype video composition instruction.

Deprecated

init(asset: AVAsset, applyingCIFiltersWithHandler: (AVAsynchronousCIImageFilteringRequest) -> Void)

Creates a mutable video composition configured to apply Core Image filters to each video frame of the specified asset.

Deprecated

