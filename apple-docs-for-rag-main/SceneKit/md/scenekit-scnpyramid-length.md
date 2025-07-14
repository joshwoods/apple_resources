

- SceneKit
- SCNPyramid
-  length 

Instance Property

# length

The extent of the pyramid along its z-axis. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var length: CGFloat { get set }
```

## Discussion

The pyramid is centered in its local coordinate system, and the width and length of the pyramid are the dimensions of its rectangular base. For example, a pyramid of length `10.0` extends from `-5.0` to `5.0` along the z-axis. The default length is `1.0`. A length of zero or less creates an empty geometry.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Adjusting a Pyramid’s Dimensions

var width: CGFloat

The extent of the pyramid along its x-axis. Animatable.

var height: CGFloat

The extent of the pyramid along its y-axis. Animatable.

