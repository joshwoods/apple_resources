

- Vision
- ContoursObservation
- ContoursObservation.Contour
-  pointCount 

Instance Property

# pointCount

The contour’s number of points.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var pointCount: Int { get }
```

## See Also

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

