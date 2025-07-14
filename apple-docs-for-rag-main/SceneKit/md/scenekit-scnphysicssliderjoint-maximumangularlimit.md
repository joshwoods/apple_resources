

- SceneKit
- SCNPhysicsSliderJoint
-  maximumAngularLimit 

Instance Property

# maximumAngularLimit

The maximum rotation angle between the two bodies, measured in radians relative to their initial orientations.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var maximumAngularLimit: CGFloat { get set }
```

## Discussion

The default (and maximum) value of this property is `M_PI`. With this value, the joint can spin counterclockwise (relative to the first body) with no limit.

Set both this property and the maximumAngularLimit property to the same value to prevent the bodies from rotating around their anchor points. (Set both properties to `0.0` to fix the bodies in their initial orientations.) Bodies whose orientation is fixed by a sliding joint may still slide, depending on the values of the minimumLinearLimit and maximumLinearLimit properties.

## See Also

### Limiting the Motion of a Slider Joint

var minimumLinearLimit: CGFloat

The minimum distance between the anchor points of the two bodies, relative to their initial positions.

var maximumLinearLimit: CGFloat

The maximum distance between the anchor points of the two bodies, relative to their initial positions.

var minimumAngularLimit: CGFloat

The minimum rotation angle between the two bodies, measured in radians relative to their initial orientations.

