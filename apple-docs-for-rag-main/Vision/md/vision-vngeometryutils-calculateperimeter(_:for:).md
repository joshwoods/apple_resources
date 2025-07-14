

- Vision
- VNGeometryUtils
-  calculatePerimeter(\_:for:) 

Type Method

# calculatePerimeter(\_:for:)

Calculates the perimeter of a closed contour.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class func calculatePerimeter(
    _ perimeter: UnsafeMutablePointer,
    for contour: VNContour
) throws
```

## Parameters 

`perimeter`  

The output parameter to populate with the calculated contour perimeter.

`contour`  

The contour object for which to calculate the perimeter.

## See Also

### Calculating Area and Perimeter

class func calculateArea(UnsafeMutablePointer&lt;Double>, for: VNContour, orientedArea: Bool) throws

Calculates the area for the specified contour.

