

- Vision
- VNPoint
-  apply(\_:to:) 

Type Method

# apply(\_:to:)

Creates a point object that’s shifted by the X and Y offsets of the specified vector.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class func apply(
    _ vector: VNVector,
    to point: VNPoint
) -> VNPoint
```

## Parameters 

`vector`  

The vector to apply to offset the point.

`point`  

The point to translate by the vector’s X and Y offsets.

## See Also

### Creating a Point

init(x: Double, y: Double)

Creates a point object with the specified coordinates.

convenience init(location: CGPoint)

Creates a point object from the specified Core Graphics point.

class var zero: VNPoint

A point object that represents the origin.

