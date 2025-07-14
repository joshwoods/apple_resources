

- SceneKit
- SCNCapsule
-  capRadius 

Instance Property

# capRadius

The radius both of the capsule’s circular center cross section and of its hemispherical ends. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var capRadius: CGFloat { get set }
```

## Discussion

The capsule is centered in its local coordinate system. For example, the cylindrical body of a capsule of radius `5.0` extends from `-5.0` to `5.0` along the x- and z-axes.

If the cap radius is zero or less, or greater than half the capsule’s height, the geometry is empty. The default cap radius is `0.5`.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Adjusting a Capsule’s Dimensions

var height: CGFloat

The extent of the capsule along its y-axis. Animatable.

