

- Vision
- ContoursObservation
-  ContoursObservation.Contour 

Structure

# ContoursObservation.Contour

An object that represents a detected contour in an image.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct Contour
```

## Topics

### Inspecting a contour

var aspectRatio: Float

The aspect ratio of the contour, which is the image’s width divided by its height.

var childContours: [ContoursObservation.Contour]

An array of contours that this contour encloses.

var indexPath: IndexPath

The contour object’s index path.

var normalizedPath: CGPath

The contour object as a path in normalized coordinates.

var normalizedPoints: [simd_float2]

The contour’s array of points in normalized coordinates.

var pointCount: Int

The contour’s number of points.

### Calculating area and perimeter

func calculateArea(useOrientedArea: Bool) -> Double

func calculatePerimeter() -> Double

### Getting the bounding circle

func boundingCircle() -> NormalizedCircle

### Getting the approximation

func polygonApproximation(epsilon: Float) throws -> ContoursObservation.Contour

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Getting the contours

func contourAtIndex(Int) -> ContoursObservation.Contour?

Retrieves the contour object at the specified index, irrespective of hierarchy.

func countourAtIndexPath(IndexPath) -> ContoursObservation.Contour?

Retrieves the contour object at the specified index, irrespective of hierarchy.

