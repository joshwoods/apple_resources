

- Vision
- VNContour
-  childContours 

Instance Property

# childContours

An array of contours that this contour encloses.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var childContours: [VNContour] { get }
```

## See Also

### Accessing Child Contours

var childContourCount: Int

The total number of detected child contours.

func childContour(at: Int) throws -> VNContour

Retrieves the child contour object at the specified index.

