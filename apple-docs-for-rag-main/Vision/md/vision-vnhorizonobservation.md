

- Vision
-  VNHorizonObservation 

Class

# VNHorizonObservation

The horizon angle information that an image-analysis request detects.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class VNHorizonObservation
```

## Overview

Instances of this class result from invoking a VNDetectHorizonRequest, and report the angle and transform of the horizon in an image.

## Topics

### Evaluating the Horizon

var angle: CGFloat

The angle of the observed horizon.

var transform: CGAffineTransform

The transform to apply to the detected horizon.

func transform(forImageWidth: Int, height: Int) -> CGAffineTransform

Creates an affine transform for the specified image width and height.

## Relationships

### Inherits From

- VNObservation

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

### Horizon detection

class VNDetectHorizonRequest

An image-analysis request that determines the horizon angle in an image.

