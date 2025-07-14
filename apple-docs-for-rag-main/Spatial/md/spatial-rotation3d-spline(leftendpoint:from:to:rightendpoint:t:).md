

- Spatial
- Rotation3D
-  spline(leftEndpoint:from:to:rightEndpoint:t:) 

Type Method

# spline(leftEndpoint:from:to:rightEndpoint:t:)

Returns an interpolated value between two rotations along a spherical cubic spline.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOSwatchOS 11.0+

``` source
static func spline(
    leftEndpoint r0: Rotation3D,
    from r1: Rotation3D,
    to r2: Rotation3D,
    rightEndpoint r3: Rotation3D,
    t: Double
) -> Rotation3D
```

