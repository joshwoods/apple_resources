

- SceneKit
- SCNTube
-  init(innerRadius:outerRadius:height:) 

Initializer

# init(innerRadius:outerRadius:height:)

Creates a tube geometry with the specified inner radius, outer radius, and height.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
convenience init(
    innerRadius: CGFloat,
    outerRadius: CGFloat,
    height: CGFloat
)
```

## Parameters 

`innerRadius`  

The radius of the tube’s circular central hole in the x- and z-axes of its local coordinate space.

`outerRadius`  

The radius of the tube’s circular cross section in the x- and z-axes of its local coordinate space.

`height`  

The height of the tube along the y-axis of its local coordinate space.

## Return Value

A new tube geometry.

## Discussion

The tube is centered in its local coordinate system. For example, if you create a tube whose outer radius is `5.0`, inner radius is `1.0`, and height is `10.0`, its circular cross section extends from `-5.0` to `5.0` along the x- and z-axes, the y-coordinates of its base and top are `-5.0` and `5.0`, and the hole through its center extends from `-0.5` to `0.5` along the x- and z-axes.

