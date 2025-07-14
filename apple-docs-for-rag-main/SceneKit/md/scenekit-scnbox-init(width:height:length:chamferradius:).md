

- SceneKit
- SCNBox
-  init(width:height:length:chamferRadius:) 

Initializer

# init(width:height:length:chamferRadius:)

Creates a box geometry with the specified width, height, length, and chamfer radius.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
convenience init(
    width: CGFloat,
    height: CGFloat,
    length: CGFloat,
    chamferRadius: CGFloat
)
```

## Parameters 

`width`  

The width of the box along the x-axis of its local coordinate space.

`height`  

The height of the box along the y-axis of its local coordinate space.

`length`  

The length of the box along the z-axis of its local coordinate space.

`chamferRadius`  

The radius of curvature for the edges and corners of the box.

## Return Value

A new box geometry.

## Discussion

The box is centered in its local coordinate system. For example, if you create a box whose width, height and length are all `10.0`, it extends from `-5.0` to `5.0` along in each of the x-, y-, and z-axes.

