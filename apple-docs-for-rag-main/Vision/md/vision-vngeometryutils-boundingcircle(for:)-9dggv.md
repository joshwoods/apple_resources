

- Vision
- VNGeometryUtils
-  boundingCircle(for:) 

Type Method

# boundingCircle(for:)

Calculates a bounding circle for the specified array of points.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class func boundingCircle(for points: [VNPoint]) throws -> VNCircle
```

## Parameters 

`points`  

A collection of points around which to calculate the bounding circle.

## Return Value

The bounding VNCircle object.

## See Also

### Calculating Bounding Circles

class func boundingCircle(for: VNContour) throws -> VNCircle

Calculates a bounding circle for the specified contour object.

class func boundingCircle(forSIMDPoints: UnsafePointer&lt;simd_float2>, pointCount: Int) throws -> VNCircle

Calculates a bounding circle for the specified points.

