

- Vision
- VNCircle
-  init(center:radius:) 

Initializer

# init(center:radius:)

Creates a circle with the specified center and radius.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
init(
    center: VNPoint,
    radius: Double
)
```

## Parameters 

`center`  

The circle center.

`radius`  

The circle radius.

## See Also

### Creating a Circle

convenience init(center: VNPoint, diameter: Double)

Creates a circle with the specified center and diameter.

class var zero: VNCircle

A circle object centered at the origin, with a radius of zero.

