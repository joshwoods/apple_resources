

- SceneKit
- SCNBox
-  height 

Instance Property

# height

The extent of the box along its y-axis. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var height: CGFloat { get set }
```

## Discussion

The box is centered in its local coordinate system. For example, a box of height `10.0` extends from `-5.0` to `5.0` along the y-axis. The default width is `1.0`. A height of zero or less creates an empty geometry.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Adjusting a Box’s Dimensions

var width: CGFloat

The extent of the box along its x-axis. Animatable.

var length: CGFloat

The extent of the box along its z-axis. Animatable.

