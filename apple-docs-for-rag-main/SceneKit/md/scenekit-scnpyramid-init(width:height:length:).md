

- SceneKit
- SCNPyramid
-  init(width:height:length:) 

Initializer

# init(width:height:length:)

Creates a pyramid geometry with the specified width, height, and length.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
convenience init(
    width: CGFloat,
    height: CGFloat,
    length: CGFloat
)
```

## Parameters 

`width`  

The width of the pyramid along the x-axis of its local coordinate space.

`height`  

The height of the pyramid along the y-axis of its local coordinate space.

`length`  

The length of the pyramid along the z-axis of its local coordinate space.

## Return Value

A new pyramid geometry.

## Discussion

The pyramid’s base is centered in its local coordinate system. For example, if you create a pyramid whose width, height and length are all `10.0`, its apex is at the point `{0, 10.0, 0}`, and its base lies in the plane whose y-coordinate is `0.0`, extending from `-5.0` to `5.0` along both the x- and z-axes.

