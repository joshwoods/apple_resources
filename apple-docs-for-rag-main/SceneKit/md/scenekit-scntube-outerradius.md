

- SceneKit
- SCNTube
-  outerRadius 

Instance Property

# outerRadius

The radius of the tube’s outer circular cross section. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var outerRadius: CGFloat { get set }
```

## Discussion

The tube is centered in its local coordinate system. For example, a tube whose outer radius is `5.0` extends from `-5.0` to `5.0` along the x- and z-axes. The default outer radius is `0.5`.

An outer radius of zero or less, or equal to or smaller than the inner radius, creates an empty geometry.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Adjusting a Tube’s Dimensions

var innerRadius: CGFloat

The radius of the circular hole through the tube. Animatable.

var height: CGFloat

The extent of the tube along its y-axis. Animatable.

