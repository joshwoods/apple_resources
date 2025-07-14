

- SceneKit
- SCNCylinder
-  init(radius:height:) 

Initializer

# init(radius:height:)

Creates a cylinder geometry with the specified radius and height.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
convenience init(
    radius: CGFloat,
    height: CGFloat
)
```

## Parameters 

`radius`  

The radius of the cylinder’s circular cross section in the x- and z-axis dimensions of its local coordinate space.

`height`  

The height of the cylinder along the y-axis of its local coordinate space.

## Return Value

A new cylinder geometry.

## Discussion

The cylinder is centered in its local coordinate system. For example, if you create a cylinder whose radius is `5.0` and height is `10.0`, its circular cross section extends from `-5.0` to `5.0` along the x- and z-axes, and the y-coordinates of its base and top are `-5.0` and `5.0`, respectively.

