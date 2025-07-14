

- AVFoundation
- AVMutableVideoComposition
-  videoComposition(withPropertiesOf:prototypeInstruction:completionHandler:) 

Type Method

# videoComposition(withPropertiesOf:prototypeInstruction:completionHandler:)

Returns a new mutable video composition with the specified asset properties and a prototype video composition instruction.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
class func videoComposition(
    withPropertiesOf asset: AVAsset,
    prototypeInstruction: AVVideoCompositionInstruction,
    completionHandler: @escaping (AVMutableVideoComposition?, (any Error)?) -> Void
)
```

``` source
class func videoComposition(
    withPropertiesOf asset: AVAsset,
    prototypeInstruction: AVVideoCompositionInstruction
) async throws -> AVMutableVideoComposition
```

## Parameters 

`asset`  

The asset for which to create a video composition. Load the asset’s duration and tracks properties before invoking this method.

`prototypeInstruction`  

A video composition instruction to use as a prototype.

`completionHandler`  

A block the system calls when it finishes creating the new video composition.

## See Also

### Creating a Video Composition

class func videoComposition(withPropertiesOf: AVAsset, completionHandler: (AVMutableVideoComposition?, (any Error)?) -> Void)

Returns a new video composition that’s configured to present the video tracks of the specified asset.

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

