

- Vision
-  VNContour 

Class

# VNContour

A class that represents a detected contour in an image.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class VNContour
```

## Topics

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

func polygonApproximation(epsilon: Float) throws -> VNContour

Simplifies the contour to a polygon using a Ramer-Douglas-Peucker algorithm.

### Accessing Child Contours

var childContourCount: Int

The total number of detected child contours.

var childContours: [VNContour]

An array of contours that this contour encloses.

func childContour(at: Int) throws -> VNContour

Retrieves the child contour object at the specified index.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- VNRequestRevisionProviding

## See Also

### Inspecting the Observation

var contourCount: Int

The total number of detected contours.

var normalizedPath: CGPath

The detected contours as a path object in normalized coordinates.

var topLevelContours: [VNContour]

An array of contours that don’t have another contour enclosing them.

var topLevelContourCount: Int

The total number of detected top-level contours.

func contour(at: Int) throws -> VNContour

Retrieves the contour object at the specified index, irrespective of hierarchy.

func contour(at: IndexPath) throws -> VNContour

Retrieves the contour object at the specified index path.

