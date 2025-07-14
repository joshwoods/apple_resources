

- SceneKit
- SCNCylinder
-  radius 

Instance Property

# radius

The radius of the cylinder’s circular cross section. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var radius: CGFloat { get set }
```

## Discussion

The cylinder is centered in its local coordinate system. For example, a cylinder of radius `5.0` extends from `-5.0` to `5.0` along the x- and z-axes. The default radius is `0.5`. A radius of zero or less creates an empty geometry.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Related Documentation

class SCNCylinder

A right circular cylinder geometry.

### Adjusting a Cylinder’s Dimensions

var height: CGFloat

The extent of the cylinder along its y-axis. Animatable.

