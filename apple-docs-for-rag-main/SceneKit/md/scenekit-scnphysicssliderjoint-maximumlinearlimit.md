

- SceneKit
- SCNPhysicsSliderJoint
-  maximumLinearLimit 

Instance Property

# maximumLinearLimit

The maximum distance between the anchor points of the two bodies, relative to their initial positions.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var maximumLinearLimit: CGFloat { get set }
```

## Discussion

The default value of this property is `INFINITY`. With this value, the joint can slide forever in the direction of the slider axis.

Set both this property and the minimumLinearLimit property to the same value to pin the bodies together at their anchor points. (Set both properties to `0.0` to pin the bodies together at their initial positions.) Bodies pinned together by a sliding joint may still rotate, depending on the values of the minimumAngularLimit and maximumAngularLimit properties.

## See Also

### Limiting the Motion of a Slider Joint

var minimumLinearLimit: CGFloat

The minimum distance between the anchor points of the two bodies, relative to their initial positions.

var minimumAngularLimit: CGFloat

The minimum rotation angle between the two bodies, measured in radians relative to their initial orientations.

var maximumAngularLimit: CGFloat

The maximum rotation angle between the two bodies, measured in radians relative to their initial orientations.

