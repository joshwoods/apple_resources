

- SceneKit
- SCNCapsule
-  init(capRadius:height:) 

Initializer

# init(capRadius:height:)

Creates a capsule geometry with the specified radius and height.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
convenience init(
    capRadius: CGFloat,
    height: CGFloat
)
```

## Parameters 

`capRadius`  

The radius both of the capsule’s cylindrical body and of its hemispherical ends.

`height`  

The height of the capsule along the y-axis of its local coordinate space.

## Return Value

A new capsule geometry.

## Discussion

The capsule is centered in its local coordinate system. For example, if you create a capsule whose cap radius is `5.0` and height is `20.0`, it extends from `-10.0` to `10.0` in the y-axis, and the circular cross section at the center of its body extends from `-5.0` to `5.0` along the x- and z-axes.

