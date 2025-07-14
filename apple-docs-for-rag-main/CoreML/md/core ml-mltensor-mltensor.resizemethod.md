

- Core ML
- MLTensor
-  MLTensor.ResizeMethod 

Enumeration

# MLTensor.ResizeMethod

A resize algorithm.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
enum ResizeMethod
```

## Topics

### Enumeration Cases

case bilinear(alignCorners: Bool)

The bilinear interpolation mode where values are computed using bilinear interpolation of 4 neighboring pixels.

case nearestNeighbor

The nearest interpolation mode where values are interpolated using the closest neighbor pixel.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Hashable
- Sendable

