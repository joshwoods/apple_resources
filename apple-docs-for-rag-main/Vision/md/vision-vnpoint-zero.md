

- Vision
- VNPoint
-  zero 

Type Property

# zero

A point object that represents the origin.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class var zero: VNPoint { get }
```

## Discussion

The origin point is (0.0, 0.0).

## See Also

### Creating a Point

init(x: Double, y: Double)

Creates a point object with the specified coordinates.

convenience init(location: CGPoint)

Creates a point object from the specified Core Graphics point.

class func apply(VNVector, to: VNPoint) -> VNPoint

Creates a point object that’s shifted by the X and Y offsets of the specified vector.

