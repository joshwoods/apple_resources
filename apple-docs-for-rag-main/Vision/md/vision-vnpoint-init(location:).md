

- Vision
- VNPoint
-  init(location:) 

Initializer

# init(location:)

Creates a point object from the specified Core Graphics point.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
convenience init(location: CGPoint)
```

## Parameters 

`location`  

The Core Graphics point.

## See Also

### Creating a Point

init(x: Double, y: Double)

Creates a point object with the specified coordinates.

class func apply(VNVector, to: VNPoint) -> VNPoint

Creates a point object that’s shifted by the X and Y offsets of the specified vector.

class var zero: VNPoint

A point object that represents the origin.

