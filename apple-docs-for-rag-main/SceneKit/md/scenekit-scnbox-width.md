

- SceneKit
- SCNBox
-  width 

Instance Property

# width

The extent of the box along its x-axis. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var width: CGFloat { get set }
```

## Discussion

The box is centered in its local coordinate system. For example, a box of width `10.0` extends from `-5.0` to `5.0` along the x-axis. The default width is `1.0`. A width of zero or less creates an empty geometry.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Adjusting a Box’s Dimensions

var height: CGFloat

The extent of the box along its y-axis. Animatable.

var length: CGFloat

The extent of the box along its z-axis. Animatable.

