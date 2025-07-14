

- SceneKit
- SCNBox
-  chamferSegmentCount 

Instance Property

# chamferSegmentCount

The number of line segments used to create each rounded edge of the box. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var chamferSegmentCount: Int { get set }
```

## Discussion

A larger number of segments adds more vertex data to the geometry, creating a smoother curve for each rounded edge and corner at a cost to rendering performance.

The default corner segment count is `10`. Setting this property’s value to a number less than `1` results in undefined behavior.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Related Documentation

var heightSegmentCount: Int

The number of subdivisions in each face of the box along its y-axis. Animatable.

var widthSegmentCount: Int

The number of subdivisions in each face of the box along its x-axis. Animatable.

var lengthSegmentCount: Int

The number of subdivisions in each face of the box along its z-axis. Animatable.

### Adding Rounded Edges and Corners

var chamferRadius: CGFloat

The radius of curvature for the edges and corners of the box. Animatable.

