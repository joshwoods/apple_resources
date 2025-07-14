

- Vision
- VNGeometryUtils
-  boundingCircle(forSIMDPoints:pointCount:) 

Type Method

# boundingCircle(forSIMDPoints:pointCount:)

Calculates a bounding circle for the specified points.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class func boundingCircle(
    forSIMDPoints points: UnsafePointer,
    pointCount: Int
) throws -> VNCircle
```

## Parameters 

`points`  

A collection of points around which to calculate the bounding circle.

`pointCount`  

The number of points in the `points` argument.

## Return Value

The bounding VNCircle object.

## See Also

### Calculating Bounding Circles

class func boundingCircle(for: VNContour) throws -> VNCircle

Calculates a bounding circle for the specified contour object.

class func boundingCircle(for: [VNPoint]) throws -> VNCircle

Calculates a bounding circle for the specified array of points.

