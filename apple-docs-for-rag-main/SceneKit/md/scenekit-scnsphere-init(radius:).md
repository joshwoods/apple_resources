

- SceneKit
- SCNSphere
-  init(radius:) 

Initializer

# init(radius:)

Creates a sphere geometry with the specified radius.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
convenience init(radius: CGFloat)
```

## Parameters 

`radius`  

The radius of the sphere in its local coordinate space.

## Return Value

A new sphere geometry.

## Discussion

The sphere is centered in its local coordinate system. For example, if you create a sphere whose radius is `5.0`, it extends from `-5.0` to `5.0` along each of the the x, y, and z-axes.

