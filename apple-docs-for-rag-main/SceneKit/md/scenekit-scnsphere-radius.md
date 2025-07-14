

- SceneKit
- SCNSphere
-  radius 

Instance Property

# radius

The radius of the sphere. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var radius: CGFloat { get set }
```

## Discussion

The sphere is centered in its local coordinate system. For example, if you create a sphere whose radius is `5.0`, it extends from `-5.0` to `5.0` along each of the the x, y, and z-axes. A radius of zero or less creates an empty geometry.

You can animate changes to this property’s value. See Animating SceneKit Content.

