

- SceneKit
- SCNPlane
-  width 

Instance Property

# width

The extent of the plane along its horizontal axis. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var width: CGFloat { get set }
```

## Discussion

The plane is centered in its local coordinate system. For example, a plane of width `10.0` extends from `-5.0` to `5.0` along the x-axis. The default width is `1.0`. A width of zero or less creates an empty geometry.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Adjusting a Plane’s Dimensions

var height: CGFloat

The extent of the plane along its vertical axis. Animatable.

