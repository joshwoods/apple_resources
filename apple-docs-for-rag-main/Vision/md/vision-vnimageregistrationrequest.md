

- Vision
-  VNImageRegistrationRequest 

Class

# VNImageRegistrationRequest

The abstract superclass for image-analysis requests that align images according to their content.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class VNImageRegistrationRequest
```

## Overview

This abstract superclass forms the basis of image alignment or registration requests. Make specific requests through one of its subclasses, VNTranslationalImageRegistrationRequest or VNHomographicImageRegistrationRequest. Don’t create an instance of this superclass yourself.

## Relationships

### Inherits From

- VNTargetedImageRequest

### Inherited By

- VNHomographicImageRegistrationRequest
- VNTranslationalImageRegistrationRequest

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Image alignment

Aligning Similar Images

Construct a composite image from images that capture the same scene.

class VNTargetedImageRequest

The abstract superclass for image analysis requests that operate on both the processed image and a secondary image.

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

class VNImageTranslationAlignmentObservation

Affine transform information that an image-alignment request produces.

class VNImageHomographicAlignmentObservation

An object that represents a perspective warp transformation.

