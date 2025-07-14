

- Vision
- VNContoursObservation
-  topLevelContourCount 

Instance Property

# topLevelContourCount

The total number of detected top-level contours.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var topLevelContourCount: Int { get }
```

## See Also

### Inspecting the Observation

var contourCount: Int

The total number of detected contours.

var normalizedPath: CGPath

The detected contours as a path object in normalized coordinates.

var topLevelContours: [VNContour]

An array of contours that don’t have another contour enclosing them.

func contour(at: Int) throws -> VNContour

Retrieves the contour object at the specified index, irrespective of hierarchy.

func contour(at: IndexPath) throws -> VNContour

Retrieves the contour object at the specified index path.

class VNContour

A class that represents a detected contour in an image.

