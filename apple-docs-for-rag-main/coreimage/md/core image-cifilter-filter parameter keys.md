

- Core Image
- CIFilter
-  Filter Parameter Keys 

API Collection

# Filter Parameter Keys

Keys for input parameters to filters.

## Overview

These keys represent some of the most commonly used input parameters. A filter can use other kinds of input parameters.

## Topics

### Constants

let kCIOutputImageKey: String

A key for the CIImage object produced by a filter.

let kCIInputAmountKey: String

let kCIInputBackgroundImageKey: String

A key for the CIImage object to use as a background image.

let kCIInputImageKey: String

A key for the CIImage object to use as an input image. For filters that also use a background image, this key refers to the foreground image.

let kCIInputTimeKey: String

A key for z scalar value (NSNumber) that specifies a time.

let kCIInputDepthImageKey: String

A key for an image with depth values.

let kCIInputDisparityImageKey: String

A key for an image with disparity values.

let kCIInputTransformKey: String

A key for an NSAffineTransform object that specifies a transformation to apply.

let kCIInputScaleKey: String

A key for a scalar value (NSNumber) that specifies the amount of the effect.

let kCIInputAspectRatioKey: String

A key for a scalar value (NSNumber) that specifies a ratio.

let kCIInputCenterKey: String

A key for a CIVector object that specifies the center of the area, as *x* and *y*- coordinates, to be filtered.

let kCIInputRadiusKey: String

A key for a scalar value (NSNumber) that specifies the distance from the center of an effect.

let kCIInputAngleKey: String

A key for a scalar value (NSNumber) that specifies an angle.

let kCIInputRefractionKey: String

A key for a scalar value (NSNumber) that specifies the index of refraction of the material (such as glass) used in the effect.

let kCIInputWidthKey: String

A key for a scalar value (NSNumber) that specifies the width of the effect.

let kCIInputSharpnessKey: String

A key for a scalar value (NSNumber) that specifies the amount of sharpening to apply.

let kCIInputIntensityKey: String

A key for a scalar value (NSNumber) that specifies an intensity value.

let kCIInputEVKey: String

A key for a scalar value (NSNumber) that specifies how many F-stops brighter or darker the image should be.

let kCIInputSaturationKey: String

A key for a scalar value (NSNumber) that specifies the amount to adjust the saturation.

let kCIInputColorKey: String

A key for a CIColor object that specifies a color value.

let kCIInputBrightnessKey: String

A key for a scalar value (NSNumber) that specifies a brightness level.

let kCIInputContrastKey: String

A key for a scalar value (NSNumber) that specifies a contrast level.

let kCIInputWeightsKey: String

A key for a CIVector object that describes a weight matrix for use with a convolution filter.

let kCIInputGradientImageKey: String

A key for a CIImage object that specifies an environment map with alpha. Typically, this image contains highlight and shadow.

let kCIInputMaskImageKey: String

A key for a CIImage object to use as a mask.

let kCIInputMatteImageKey: String

let kCIInputShadingImageKey: String

A key for a CIImage object that specifies an environment map with alpha values. Typically this image contains highlight and shadow.

let kCIInputTargetImageKey: String

A key for a CIImage object that is the target image for a transition.

let kCIInputExtentKey: String

A key for a CIVector object that specifies a rectangle that defines the extent of the effect.

let kCIInputVersionKey: String

A key for an NSNumber object that specifies a version number.

static let baselineExposure: CIRAWFilterOption

A key for an NSNumber object containing a float that expresses the amount of baseline exposure applied to an image.

Deprecated

static let disableGamutMap: CIRAWFilterOption

A key for an NSNumber object containing a Boolean value that determines whether or not to disable gamut mapping.

Deprecated

static let moireAmount: CIRAWFilterOption

A key for an NSNumber object containing a double that expresses the amount of moiré reduction applied to an image.

Deprecated

