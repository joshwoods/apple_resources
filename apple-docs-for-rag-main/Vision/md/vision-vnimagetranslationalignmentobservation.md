

- Vision
-  VNImageTranslationAlignmentObservation 

Class

# VNImageTranslationAlignmentObservation

Affine transform information that an image-alignment request produces.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class VNImageTranslationAlignmentObservation
```

## Overview

This type of observation results from a VNTranslationalImageRegistrationRequest, informing the alignmentTransform performed to align the input images.

## Topics

### Determining Alignment

var alignmentTransform: CGAffineTransform

The alignment transform to align the floating image with the reference image.

### Identifying Request Revisions

let VNTranslationalImageRegistrationRequestRevision1: Int

A constant for specifying revision 1 of the translational image registration request.

## Relationships

### Inherits From

- VNImageAlignmentObservation

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- VNRequestRevisionProviding

## See Also

### Image alignment

Aligning Similar Images

Construct a composite image from images that capture the same scene.

class VNTargetedImageRequest

The abstract superclass for image analysis requests that operate on both the processed image and a secondary image.

class VNImageRegistrationRequest

The abstract superclass for image-analysis requests that align images according to their content.

class VNTranslationalImageRegistrationRequest

An image-analysis request that determines the affine transform necessary to align the content of two images.

class VNTrackTranslationalImageRegistrationRequest

An image-analysis request, as a stateful request you track over time, that determines the affine transform necessary to align the content of two images.

class VNHomographicImageRegistrationRequest

An image-analysis request that determines the perspective warp matrix necessary to align the content of two images.

class VNTrackHomographicImageRegistrationRequest

An image-analysis request, as a stateful request you track over time, that determines the perspective warp matrix necessary to align the content of two images.

class VNImageAlignmentObservation

The abstract superclass for image-analysis results that describe the relative alignment of two images.

class VNImageHomographicAlignmentObservation

An object that represents a perspective warp transformation.

