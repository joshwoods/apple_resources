

- Vision
- VNContoursObservation
-  contour(at:) 

Instance Method

# contour(at:)

Retrieves the contour object at the specified index path.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func contour(at indexPath: IndexPath) throws -> VNContour
```

## Parameters 

`indexPath`  

The hierarchical index path to the contour.

## Return Value

The contour object at the specified index path.

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

class VNContour

A class that represents a detected contour in an image.

