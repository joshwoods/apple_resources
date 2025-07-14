

- Vision
- VNContoursObservation
-  topLevelContours 

Instance Property

# topLevelContours

An array of contours that don’t have another contour enclosing them.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var topLevelContours: [VNContour] { get }
```

## Discussion

This array constitutes the top of the contour hierarchy. You can iterate over each VNContour instance to determine its children.

## See Also

### Inspecting the Observation

var contourCount: Int

The total number of detected contours.

var normalizedPath: CGPath

The detected contours as a path object in normalized coordinates.

var topLevelContourCount: Int

The total number of detected top-level contours.

func contour(at: Int) throws -> VNContour

Retrieves the contour object at the specified index, irrespective of hierarchy.

func contour(at: IndexPath) throws -> VNContour

Retrieves the contour object at the specified index path.

class VNContour

A class that represents a detected contour in an image.

