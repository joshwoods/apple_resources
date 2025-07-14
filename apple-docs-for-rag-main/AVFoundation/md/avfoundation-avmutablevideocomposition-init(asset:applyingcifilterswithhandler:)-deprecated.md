

- AVFoundation
- AVMutableVideoComposition
-  init(asset:applyingCIFiltersWithHandler:) Deprecated

Initializer

# init(asset:applyingCIFiltersWithHandler:)

Creates a mutable video composition configured to apply Core Image filters to each video frame of the specified asset.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 9.0–18.0Deprecated

``` source
init(
    asset: AVAsset,
    applyingCIFiltersWithHandler applier: @escaping (AVAsynchronousCIImageFilteringRequest) -> Void
)
```

Deprecated

Use videoCompositionWithAsset:applyingCIFiltersWithHandler:completionHandler: instead

## Parameters 

`asset`  

The asset whose configuration matches the intended use of the video composition.

`applier`  

A block that AVFoundation calls when processing each video frame.

The block takes a single parameter and has no return value:

request  
An AVAsynchronousCIImageFilteringRequest object representing the frame to be processed.

## Return Value

A new video composition object.

## Discussion

To process video frames using Core Image filters—whether for display or export—create a composition with this method. AVFoundation calls your applier block once for each frame to be displayed (or processed for export) from the asset’s first enabled video track. In that block, you access the video frame and return a filtered result using the provided AVAsynchronousCIImageFilteringRequest object. Use that object’s sourceImage property to get the video frame in the form of a CIImage object you can apply filters to. Pass the result of your filters to the `request` object’s finish(with:context:) method. (If your filter rendering fails, call the `request` object’s finish(with:) method if you cannot apply filters.)

Creating a composition with this method sets values for the following properties:

- The frameDuration property is set to accommodate the nominalFrameRate value for the asset’s first enabled video track. If the nominal frame rate is zero, AVFoundation uses a default framerate of 30 fps.

- The renderSize property is set to a size that encompasses the asset’s first enabled video track, respecting the track’s preferredTransform property.

- The animationTool property is set to `1.0`.

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

init(propertiesOf: AVAsset, prototypeInstruction: AVVideoCompositionInstruction)

Creates a mutable video composition with the specified asset properties and a prototype video composition instruction.

Deprecated

