

- Vision
- VNContour
-  aspectRatio 

Instance Property

# aspectRatio

The aspect ratio of the contour.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var aspectRatio: Float { get }
```

## Discussion

The aspect ratio is the original image’s width divided by its height.

## See Also

### Inspecting the Contour

var indexPath: IndexPath

The contour object’s index path.

var normalizedPath: CGPath

The contour object as a path in normalized coordinates.

var pointCount: Int

The contour’s number of points.

var normalizedPoints: [simd_float2]

The contour’s array of points in normalized coordinates.

func polygonApproximation(epsilon: Float) throws -> VNContour

Simplifies the contour to a polygon using a Ramer-Douglas-Peucker algorithm.

