

- Vision
- VNGenerateImageFeaturePrintRequest
-  imageCropAndScaleOption 

Instance Property

# imageCropAndScaleOption

An optional setting that tells the algorithm how to scale an input image before generating the feature print.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
var imageCropAndScaleOption: VNImageCropAndScaleOption { get set }
```

## Discussion

Scaling is applied before generating the feature print. The default value is VNImageCropAndScaleOption.scaleFill.

Scaling an image ensures that the entire image fits into the algorithm’s input image dimensions, which may require a change in aspect ratio. Each crop and scale option transforms the input image in a different way:

## See Also

### Scaling and Cropping Images

enum VNImageCropAndScaleOption

Options that define how Vision crops and scales an input-image.

