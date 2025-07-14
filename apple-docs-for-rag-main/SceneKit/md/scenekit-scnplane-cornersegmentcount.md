

- SceneKit
- SCNPlane
-  cornerSegmentCount 

Instance Property

# cornerSegmentCount

The number of line segments used to create each rounded corner of the plane. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
var cornerSegmentCount: Int { get set }
```

## Discussion

A larger number of segments adds more vertex data to the geometry, creating a smoother curve for each rounded corner at a cost to rendering performance.

The default corner segment count is `10`. Setting this property’s value to a number less than `1` results in undefined behavior.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Related Documentation

var heightSegmentCount: Int

The number of subdivisions in the plane’s surface along its vertical axis. Animatable.

var widthSegmentCount: Int

The number of subdivisions in the plane’s surface along its horizontal axis. Animatable.

### Adding Rounded Corners

var cornerRadius: CGFloat

The radius of curvature for the plane’s corners. Animatable.

