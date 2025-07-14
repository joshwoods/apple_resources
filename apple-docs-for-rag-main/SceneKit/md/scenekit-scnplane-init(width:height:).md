

- SceneKit
- SCNPlane
-  init(width:height:) 

Initializer

# init(width:height:)

Creates a plane geometry with the specified width and height.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
convenience init(
    width: CGFloat,
    height: CGFloat
)
```

## Parameters 

`width`  

The width of the plane along the x-axis of its local coordinate space.

`height`  

The height of the plane along the y-axis of its local coordinate space.

## Return Value

A new plane geometry.

## Discussion

The plane is centered in its local coordinate system. For example, if you create a plane whose width and height are both `10.0`, it extends from `-5.0` to `5.0` along both the x- and y-axes, and the z-coordinate of all points in the plane is zero.

