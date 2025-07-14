

- Vision
- VNContour
-  normalizedPath 

Instance Property

# normalizedPath

The contour object as a path in normalized coordinates.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var normalizedPath: CGPath { get }
```

## See Also

### Inspecting the Contour

var aspectRatio: Float

The aspect ratio of the contour.

var indexPath: IndexPath

The contour object’s index path.

var pointCount: Int

The contour’s number of points.

var normalizedPoints: [simd_float2]

The contour’s array of points in normalized coordinates.

func polygonApproximation(epsilon: Float) throws -> VNContour

Simplifies the contour to a polygon using a Ramer-Douglas-Peucker algorithm.

