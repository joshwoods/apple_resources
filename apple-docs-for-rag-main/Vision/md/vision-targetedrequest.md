

- Vision
-  TargetedRequest 

Protocol

# TargetedRequest

A type for analyzing two images together.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
protocol TargetedRequest : VisionRequest
```

## Relationships

### Inherits From

- CustomStringConvertible
- Equatable
- Hashable
- Sendable
- VisionRequest

### Conforming Types

- TrackHomographicImageRegistrationRequest
- TrackOpticalFlowRequest
- TrackTranslationalImageRegistrationRequest

## See Also

### Image alignment

class TrackTranslationalImageRegistrationRequest

An image-analysis request that you track over time to determine the affine transform necessary to align the content of two images.

class TrackHomographicImageRegistrationRequest

An image-analysis request that you track over time to determine the perspective warp matrix necessary to align the content of two images.

