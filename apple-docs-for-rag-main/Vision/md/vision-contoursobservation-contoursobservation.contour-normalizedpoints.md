

- Vision
- ContoursObservation
- ContoursObservation.Contour
-  normalizedPoints 

Instance Property

# normalizedPoints

The contour’s array of points in normalized coordinates.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var normalizedPoints: [simd_float2] { get }
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

var pointCount: Int

The contour’s number of points.

