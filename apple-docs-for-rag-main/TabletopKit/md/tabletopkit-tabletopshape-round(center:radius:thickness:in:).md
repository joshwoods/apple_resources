

- TabletopKit
- TabletopShape
-  round(center:radius:thickness:in:) 

Type Method

# round(center:radius:thickness:in:)

Creates a round tabletop shape with the specified center, radius, and thickness.

visionOS 2.0+

``` source
static func round(
    center: Point3D = .zero,
    radius: Float,
    thickness: Float,
    in unit: UnitLength = .meters
) -> TabletopShape
```

## See Also

### Creating a round or rectangular table

static func rectangular(center: Point3D, width: Float, height: Float, thickness: Float, in: UnitLength) -> TabletopShape

Creates a rectangular tabletop shape with the specified center and dimensions.

