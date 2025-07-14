

- Vision
- VNGeometryUtils
-  calculateArea(\_:for:orientedArea:) 

Type Method

# calculateArea(\_:for:orientedArea:)

Calculates the area for the specified contour.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class func calculateArea(
    _ area: UnsafeMutablePointer,
    for contour: VNContour,
    orientedArea: Bool
) throws
```

## Parameters 

`area`  

The output parameter to populate with the calculated contour area.

`contour`  

The contour object for which to calculate the area.

`orientedArea`  

A Boolean value that indicates whether to calculate the signed area (positive for counterclockwise-oriented contours and negative for clockwise-oriented contours). If you specify false, the returned area is always positive.

## Discussion

Attempting to calculate the area for a contour containing random points, or with self-crossing edges, produces undefined results.

## See Also

### Calculating Area and Perimeter

class func calculatePerimeter(UnsafeMutablePointer&lt;Double>, for: VNContour) throws

Calculates the perimeter of a closed contour.

