

- AVFoundation
- AVVideoComposition
-  videoComposition(with:applyingCIFiltersWithHandler:completionHandler:) 

Type Method

# videoComposition(with:applyingCIFiltersWithHandler:completionHandler:)

Returns a new video composition that’s configured to apply Core Image filters to each video frame of the specified asset.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
class func videoComposition(
    with asset: AVAsset,
    applyingCIFiltersWithHandler applier: @escaping (AVAsynchronousCIImageFilteringRequest) -> Void,
    completionHandler: @escaping (AVVideoComposition?, (any Error)?) -> Void
)
```

``` source
class func videoComposition(
    with asset: AVAsset,
    applyingCIFiltersWithHandler applier: @escaping (AVAsynchronousCIImageFilteringRequest) -> Void
) async throws -> AVVideoComposition
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

```
guard let filter = CIFilter(name: "CIGaussianBlur") else { return }
let composition = try await AVVideoComposition.videoComposition(with: asset) { request in
    // Clamp to avoid blurring transparent pixels at the image edges.
    let source = request.sourceImage.clampedToExtent()
    filter.setValue(source, forKey: kCIInputImageKey)

    // Vary filter parameters based on the video timing.
    let seconds = CMTimeGetSeconds(request.compositionTime)
    filter.setValue(seconds * 10.0, forKey: kCIInputRadiusKey)

    // Crop the blurred output to the bounds of the original image.
    if let output = filter.outputImage?.cropped(to: request.sourceImage.extent) {
        request.finish(with: output, context: nil)
    } else {
        request.finish(with: AppError.customError)
    }
}
```

Creating a composition with this method sets values for the following properties:

- The value of the frameDuration property accommodates the nominalFrameRate value for the asset’s first enabled video track. If the nominal frame rate is zero, AVFoundation uses a default frame rate of 30 fps.

- The renderSize property value a size that encompasses the asset’s first enabled video track, respecting the track’s preferredTransform property.

- The renderScale property value is `1.0`.

## See Also

### Creating a Video Composition

class func videoComposition(withPropertiesOf: AVAsset, completionHandler: (AVVideoComposition?, (any Error)?) -> Void)

Returns a new video composition that’s configured to present the video tracks of the specified asset.

class AVAsynchronousCIImageFilteringRequest

An object that supports using Core Image filters to process an individual video frame in a video composition.

init(propertiesOf: AVAsset)

Creates a video composition object configured to present the video tracks of the specified asset.

Deprecated

init(asset: AVAsset, applyingCIFiltersWithHandler: (AVAsynchronousCIImageFilteringRequest) -> Void)

Creates a video composition configured to apply Core Image filters to each video frame of the specified asset.

Deprecated

