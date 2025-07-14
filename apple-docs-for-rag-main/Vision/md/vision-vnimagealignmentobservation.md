

- Vision
-  VNImageAlignmentObservation 

Class

# VNImageAlignmentObservation

The abstract superclass for image-analysis results that describe the relative alignment of two images.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class VNImageAlignmentObservation
```

## Overview

This abstract superclass forms the basis of image alignment or registration output. You receive its subclasses, such as VNImageTranslationAlignmentObservation and VNImageHomographicAlignmentObservation, by performing specific registration requests. Don’t create one of these classes yourself.

## Relationships

### Inherits From

- VNObservation

### Inherited By

- VNImageHomographicAlignmentObservation
- VNImageTranslationAlignmentObservation

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

class VNImageTranslationAlignmentObservation

Affine transform information that an image-alignment request produces.

class VNImageHomographicAlignmentObservation

An object that represents a perspective warp transformation.

