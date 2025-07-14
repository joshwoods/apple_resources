

- SceneKit
- SCNBox
-  widthSegmentCount 

Instance Property

# widthSegmentCount

The number of subdivisions in each face of the box along its x-axis. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var widthSegmentCount: Int { get set }
```

## Discussion

A larger number of segments adds more vertex data to the geometry. Although each face of the box is a flat plane, extra vertices can be useful for lighting or custom shader programs. Adding vertices increases rendering cost, so use the minimal segment count that produces your desired visual effect.

The default segment count is `1`. Setting this property’s value to a number less than `1` results in undefined behavior. If the chamferRadius property’s value is greater than zero, the segment count applies only to the flat faces between chamfered edges.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Configuring Box Properties

var heightSegmentCount: Int

The number of subdivisions in each face of the box along its y-axis. Animatable.

var lengthSegmentCount: Int

The number of subdivisions in each face of the box along its z-axis. Animatable.

