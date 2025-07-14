

- TabletopKit
- TabletopShape
-  rectangular(center:width:height:thickness:in:) 

Type Method

# rectangular(center:width:height:thickness:in:)

Creates a rectangular tabletop shape with the specified center and dimensions.

visionOS 2.0+

``` source
static func rectangular(
    center: Point3D = .zero,
    width: Float,
    height: Float,
    thickness: Float,
    in unit: UnitLength = .meters
) -> TabletopShape
```

## See Also

### Creating a round or rectangular table

static func round(center: Point3D, radius: Float, thickness: Float, in: UnitLength) -> TabletopShape

Creates a round tabletop shape with the specified center, radius, and thickness.

