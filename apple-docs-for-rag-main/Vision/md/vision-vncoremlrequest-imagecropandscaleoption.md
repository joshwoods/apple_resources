

- Vision
- VNCoreMLRequest
-  imageCropAndScaleOption 

Instance Property

# imageCropAndScaleOption

An optional setting that tells the Vision algorithm how to scale an input image.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var imageCropAndScaleOption: VNImageCropAndScaleOption { get set }
```

## Discussion

Scaling an image ensures that the entire image fits into the algorithm’s input image dimensions, which may require a change in aspect ratio. Each crop-and-scale option transforms the input image in a different way.

## See Also

### Configuring Image Options

enum VNImageCropAndScaleOption

Options that define how Vision crops and scales an input-image.

