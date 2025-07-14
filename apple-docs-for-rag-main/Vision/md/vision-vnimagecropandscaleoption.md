

- Vision
-  VNImageCropAndScaleOption 

Enumeration

# VNImageCropAndScaleOption

Options that define how Vision crops and scales an input-image.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
enum VNImageCropAndScaleOption
```

## Overview

Scaling an image ensures that it fits within the algorithm’s input image dimensions, which may require a change in aspect ratio. The figure below shows how each crop-and-scale option transforms the input image:

## Topics

### Crop and Scale Options

case centerCrop

An option that scales the image to fit its shorter side within the input dimensions, while preserving its aspect ratio, and center-crops the image.

case scaleFit

An option that scales the image to fit its longer side within the input dimensions, while preserving its aspect ratio, and center-crops the image.

case scaleFill

An option that scales the image to fill the input dimensions, resizing it if necessary.

case scaleFitRotate90CCW

An option that rotates the image 90 degrees counterclockwise and then scales it, while preserving its aspect ratio, to fit on the long side.

case scaleFillRotate90CCW

An option that rotates the image 90 degrees counterclockwise and then scales it to fill the input dimensions.

### Creating a Scale Option

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring Image Options

var imageCropAndScaleOption: VNImageCropAndScaleOption

An optional setting that tells the Vision algorithm how to scale an input image.

