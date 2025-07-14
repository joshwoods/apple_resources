

- AVFoundation
- AVMutableVideoComposition
-  init(propertiesOf:prototypeInstruction:) Deprecated

Initializer

# init(propertiesOf:prototypeInstruction:)

Creates a mutable video composition with the specified asset properties and a prototype video composition instruction.

iOS 13.0–18.0DeprecatediPadOS 13.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.15–15.0DeprecatedtvOS 13.0–18.0Deprecated

``` source
init(
    propertiesOf asset: AVAsset,
    prototypeInstruction: AVVideoCompositionInstruction
)
```

Deprecated

Use videoCompositionWithPropertiesOfAsset:prototypeInstruction:completionHandler: instead

## Parameters 

`asset`  

The asset for which to create a video composition. Load the asset’s duration and tracks properties before invoking this method.

`prototypeInstruction`  

A video composition instruction to use as a prototype.

## See Also

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

init(asset: AVAsset, applyingCIFiltersWithHandler: (AVAsynchronousCIImageFilteringRequest) -> Void)

Creates a mutable video composition configured to apply Core Image filters to each video frame of the specified asset.

Deprecated

