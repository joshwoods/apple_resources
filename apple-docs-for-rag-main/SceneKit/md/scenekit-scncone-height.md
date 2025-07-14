

- SceneKit
- SCNCone
-  height 

Instance Property

# height

The extent of the cylinder along its y-axis. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var height: CGFloat { get set }
```

## Discussion

The cone is centered in its local coordinate system. For example, if a cone has a height of `10.0`, its base lies in the plane whose y-coordinate is `-5.0` and its top has a y-coordinate of `5.0`. The default height is `1.0`. A height of zero or less creates an empty geometry.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Adjusting a Cone’s Dimensions

var topRadius: CGFloat

The radius of the cone’s circular top. Animatable.

var bottomRadius: CGFloat

The radius of the cone’s circular base. Animatable.

