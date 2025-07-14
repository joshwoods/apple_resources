

- Vision
- VNContour
-  polygonApproximation(epsilon:) 

Instance Method

# polygonApproximation(epsilon:)

Simplifies the contour to a polygon using a Ramer-Douglas-Peucker algorithm.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func polygonApproximation(epsilon: Float) throws -> VNContour
```

## Parameters 

`epsilon`  

This parameter defines the distance threshold the algorithm uses. It preserves points whose perpendicular distance to the line segment they are on is greater than `epsilon`, and removes all others.

## Return Value

A simplified polygon contour from the points of the original contour.

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

var normalizedPoints: [simd_float2]

The contour’s array of points in normalized coordinates.

