

- Vision
- VNImageCropAndScaleOption
-  VNImageCropAndScaleOption.scaleFillRotate90CCW 

Case

# VNImageCropAndScaleOption.scaleFillRotate90CCW

An option that rotates the image 90 degrees counterclockwise and then scales it to fill the input dimensions.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
case scaleFillRotate90CCW
```

## Discussion

This option optimizes portrait images to fill into landscape buffers for algorithms that are rotation agnostic.

## See Also

### Crop and Scale Options

case centerCrop

An option that scales the image to fit its shorter side within the input dimensions, while preserving its aspect ratio, and center-crops the image.

case scaleFit

An option that scales the image to fit its longer side within the input dimensions, while preserving its aspect ratio, and center-crops the image.

case scaleFill

An option that scales the image to fill the input dimensions, resizing it if necessary.

case scaleFitRotate90CCW

An option that rotates the image 90 degrees counterclockwise and then scales it, while preserving its aspect ratio, to fit on the long side.

