

- AVFoundation
- AVMutableVideoComposition
-  videoComposition(with:applyingCIFiltersWithHandler:completionHandler:) 

Type Method

# videoComposition(with:applyingCIFiltersWithHandler:completionHandler:)

Returns a new video composition that’s configured to apply Core Image filters to each video frame of the specified asset.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
class func videoComposition(
    with asset: AVAsset,
    applyingCIFiltersWithHandler applier: @escaping (AVAsynchronousCIImageFilteringRequest) -> Void,
    completionHandler: @escaping (AVMutableVideoComposition?, (any Error)?) -> Void
)
```

``` source
class func videoComposition(
    with asset: AVAsset,
    applyingCIFiltersWithHandler applier: @escaping (AVAsynchronousCIImageFilteringRequest) -> Void
) async throws -> AVMutableVideoComposition
```

## Parameters 

`asset`  

The asset whose configuration matches the intended use of the video composition.

`applier`  

A block that AVFoundation calls when processing each video frame.

The block takes a single parameter and has no return value:

request  
An AVAsynchronousCIImageFilteringRequest object representing the frame to be processed.

`completionHandler`  

A block the system calls when it finishes creating the new video composition.

## Discussion

The composition calls the specified handler one time for each frame to display (or processed for export) from the asset’s first enabled video track. In that block, you access the video frame and return a filtered result using the provided AVAsynchronousCIImageFilteringRequest object. Use that object’s sourceImage property to get the video frame in the form of a CIImage object you can apply filters to. Pass the result of your filters to the `request` object’s finish(with:context:) method. (If your filter rendering fails, call the `request` object’s finish(with:) method if you can’t apply filters).

Creating a composition with this method sets values for the following properties:

- The value of the frameDuration property accommodates the nominalFrameRate value for the asset’s first enabled video track. If the nominal frame rate is zero, AVFoundation uses a default frame rate of 30 fps.

- The renderSize property value a size that encompasses the asset’s first enabled video track, respecting the track’s preferredTransform property.

- The renderScale property value is `1.0`.

## See Also

### Creating a Video Composition

class func videoComposition(withPropertiesOf: AVAsset, completionHandler: (AVMutableVideoComposition?, (any Error)?) -> Void)

Returns a new video composition that’s configured to present the video tracks of the specified asset.

class func videoComposition(withPropertiesOf: AVAsset, prototypeInstruction: AVVideoCompositionInstruction, completionHandler: (AVMutableVideoComposition?, (any Error)?) -> Void)

Returns a new mutable video composition with the specified asset properties and a prototype video composition instruction.

init(propertiesOf: AVAsset)

Creates a mutable video composition with the specified asset properties.

Deprecated

init(propertiesOf: AVAsset, prototypeInstruction: AVVideoCompositionInstruction)

Creates a mutable video composition with the specified asset properties and a prototype video composition instruction.

Deprecated

init(asset: AVAsset, applyingCIFiltersWithHandler: (AVAsynchronousCIImageFilteringRequest) -> Void)

Creates a mutable video composition configured to apply Core Image filters to each video frame of the specified asset.

Deprecated

