

- Vision
- VNContour
-  childContourCount 

Instance Property

# childContourCount

The total number of detected child contours.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var childContourCount: Int { get }
```

## See Also

### Accessing Child Contours

var childContours: [VNContour]

An array of contours that this contour encloses.

func childContour(at: Int) throws -> VNContour

Retrieves the child contour object at the specified index.

