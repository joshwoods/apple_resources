

- SceneKit
- SCNPyramid
-  height 

Instance Property

# height

The extent of the pyramid along its y-axis. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var height: CGFloat { get set }
```

## Discussion

The pyramid’s base is centered in its local coordinate system. For example, if you create a pyramid of height `10.0`, the y-coordinate of every point in its rectangular base is `0.0` and the y-coordinate of its apex is `10.0`. The default height is `1.0`. A height of zero or less creates an empty geometry.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Adjusting a Pyramid’s Dimensions

var width: CGFloat

The extent of the pyramid along its x-axis. Animatable.

var length: CGFloat

The extent of the pyramid along its z-axis. Animatable.

