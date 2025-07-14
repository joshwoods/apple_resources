

- SceneKit
- SCNPlane
-  height 

Instance Property

# height

The extent of the plane along its vertical axis. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var height: CGFloat { get set }
```

## Discussion

The plane is centered in its local coordinate system. For example, a plane of height `10.0` extends from `-5.0` to `5.0` along the y-axis. The default height is `1.0`. A height of zero or less creates an empty geometry.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Adjusting a Plane’s Dimensions

var width: CGFloat

The extent of the plane along its horizontal axis. Animatable.

