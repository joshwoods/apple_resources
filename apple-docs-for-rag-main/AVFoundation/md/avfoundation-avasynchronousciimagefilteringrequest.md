

- AVFoundation
-  AVAsynchronousCIImageFilteringRequest 

Class

# AVAsynchronousCIImageFilteringRequest

An object that supports using Core Image filters to process an individual video frame in a video composition.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class AVAsynchronousCIImageFilteringRequest
```

## Overview

You use this class when creating a composition for Core Image filtering with the init(asset:applyingCIFiltersWithHandler:) method. In that method call, you provide a block to be called by AVFoundation as it processes each frame of video, and the block’s sole parameter is a AVAsynchronousCIImageFilteringRequest object. Use that object both to the video frame image to be filtered and allows you to return a filtered image to AVFoundation for display or export. The code listing below shows an example of applying a filter to an asset.

- Swift
- Objective-C

```
guard let filter = CIFilter(name: "CIGaussianBlur") else { return }
let composition = AVVideoComposition(asset: asset) { request in
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

```
CIFilter *filter = [CIFilter filterWithName:@"CIGaussianBlur"];
AVVideoComposition *composition = [AVVideoComposition videoCompositionWithAsset: asset
    applyingCIFiltersWithHandler:^(AVAsynchronousCIImageFilteringRequest *request){
        // Clamp to avoid blurring transparent pixels at the image edges
        CIImage *source = [request.sourceImage imageByClampingToExtent];
        [filter setValue:source forKey:kCIInputImageKey];

        // Vary filter parameters based on video timing
        Float64 seconds = CMTimeGetSeconds(request.compositionTime);
        [filter setValue:seconds * 10.0 forKey:kCIInputRadiusKey];

        // Crop the blurred output to the bounds of the original image
        CIImage *output = [filter.outputImage imageByCroppingToRect:request.sourceImage.extent];

        // Provide the filter output to the composition
        [request finishWithImage:output context:nil];
    }];
```

Tip

To use the created video composition for playback, create an AVPlayerItem object from the same asset used as the composition’s source, then assign the composition to the player item’s videoComposition property. To export the composition to a new movie file, create an AVAssetExportSession object from the same source asset, then assign the composition to the export session’s videoComposition property.

## Topics

### Getting the Image to be Filtered

var sourceImage: CIImage

The current video frame image.

### Getting Contextual Information for Filtering

var compositionTime: CMTime

The time in the video composition corresponding to the frame being processed.

var renderSize: CGSize

The width and height, in pixels, of the frame being processed.

### Returning the Filtered Image

func finish(with: CIImage, context: CIContext?)

Provides the filtered video frame image to AVFoundation for further processing or display.

func finish(with: any Error)

Notifies AVFoundation that you cannot fulfill the image filtering request.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Creating a Video Composition

class func videoComposition(withPropertiesOf: AVAsset, completionHandler: (AVVideoComposition?, (any Error)?) -> Void)

Returns a new video composition that’s configured to present the video tracks of the specified asset.

class func videoComposition(with: AVAsset, applyingCIFiltersWithHandler: (AVAsynchronousCIImageFilteringRequest) -> Void, completionHandler: (AVVideoComposition?, (any Error)?) -> Void)

Returns a new video composition that’s configured to apply Core Image filters to each video frame of the specified asset.

init(propertiesOf: AVAsset)

Creates a video composition object configured to present the video tracks of the specified asset.

Deprecated

init(asset: AVAsset, applyingCIFiltersWithHandler: (AVAsynchronousCIImageFilteringRequest) -> Void)

Creates a video composition configured to apply Core Image filters to each video frame of the specified asset.

Deprecated

