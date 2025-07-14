

- Vision
-  VNGenerateForegroundInstanceMaskRequest 

Class

# VNGenerateForegroundInstanceMaskRequest

A request that generates an instance mask of noticable objects to separate from the background.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
class VNGenerateForegroundInstanceMaskRequest
```

## Topics

### Accessing the Results

var results: [VNInstanceMaskObservation]?

The instance masks the request observes.

## Relationships

### Inherits From

- VNImageBasedRequest

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Image background removal

Applying visual effects to foreground subjects

Segment the foreground subjects of an image and composite them to a new background with visual effects.

class VNInstanceMaskObservation

An observation that contains an instance mask that labels instances in the mask.

let VNGenerateForegroundInstanceMaskRequestRevision1: Int

A constant for specifying the first revision of the foreground instance mask request.

