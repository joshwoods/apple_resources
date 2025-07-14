

- Vision
- VNContour
-  childContour(at:) 

Instance Method

# childContour(at:)

Retrieves the child contour object at the specified index.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func childContour(at childContourIndex: Int) throws -> VNContour
```

## Parameters 

`childContourIndex`  

The child contour index value.

## Return Value

The child contour object.

## See Also

### Accessing Child Contours

var childContourCount: Int

The total number of detected child contours.

var childContours: [VNContour]

An array of contours that this contour encloses.

