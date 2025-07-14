

- Vision
- VNPoint
-  init(x:y:) 

Initializer

# init(x:y:)

Creates a point object with the specified coordinates.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
init(
    x: Double,
    y: Double
)
```

## Parameters 

`x`  

The x-coordinate value.

`y`  

The y-coordinate value.

## See Also

### Creating a Point

convenience init(location: CGPoint)

Creates a point object from the specified Core Graphics point.

class func apply(VNVector, to: VNPoint) -> VNPoint

Creates a point object that’s shifted by the X and Y offsets of the specified vector.

class var zero: VNPoint

A point object that represents the origin.

