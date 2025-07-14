

- Vision
-  VNTrackTranslationalImageRegistrationRequest 

Class

# VNTrackTranslationalImageRegistrationRequest

An image-analysis request, as a stateful request you track over time, that determines the affine transform necessary to align the content of two images.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
class VNTrackTranslationalImageRegistrationRequest
```

## Overview

This request is similar to VNTranslationalImageRegistrationRequest. However, as a VNStatefulRequest, it automatically computes the registration against the previous frame.

## Topics

### Creating a Translational Image

init()

Creates a new request that tracks the translational registration of two images.

init(completionHandler: VNRequestCompletionHandler?)

Creates a new request that tracks the translational registration of two images, with a system callback on completion.

### Accessing the Results

var results: [VNImageTranslationAlignmentObservation]?

The observed translational image alignment request.

## Relationships

### Inherits From

- VNStatefulRequest

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

class VNImageRegistrationRequest

The abstract superclass for image-analysis requests that align images according to their content.

class VNTranslationalImageRegistrationRequest

An image-analysis request that determines the affine transform necessary to align the content of two images.

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

