

- Vision
- VNContour
-  normalizedPoints 

Instance Property

# normalizedPoints

The contour’s array of points in normalized coordinates.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
@nonobjc
var normalizedPoints: [simd_float2] { get }
```

## Discussion

This property value provides the address of the buffer that contain the array of CGPoint values.

## See Also

### Inspecting the Contour

var aspectRatio: Float

The aspect ratio of the contour.

var indexPath: IndexPath

The contour object’s index path.

var normalizedPath: CGPath

The contour object as a path in normalized coordinates.

var pointCount: Int

The contour’s number of points.

func polygonApproximation(epsilon: Float) throws -> VNContour

Simplifies the contour to a polygon using a Ramer-Douglas-Peucker algorithm.

