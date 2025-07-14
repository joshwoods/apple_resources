

- SceneKit
- SCNBox
-  chamferRadius 

Instance Property

# chamferRadius

The radius of curvature for the edges and corners of the box. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var chamferRadius: CGFloat { get set }
```

## Discussion

The minimum (and default) corner radius is `0.0`, specifying square corners. Set this property to a nonzero value to add rounded edges and corners to the box. Setting a corner radius of less than zero creates an empty geometry.

The maximum corner radius is half the box’s smallest dimension. For example, if a box’s width and length are both `5.0` and its height is `10.0`, its maximum corner radius is `2.5`. With these dimensions, the box’s four rounded vertical edges join to form a cylinder and its vertical faces disappear. Increasing the corner radius beyond the maximum has no visible effect.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Adding Rounded Edges and Corners

var chamferSegmentCount: Int

The number of line segments used to create each rounded edge of the box. Animatable.

