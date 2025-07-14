

- SceneKit
- SCNPyramid
-  heightSegmentCount 

Instance Property

# heightSegmentCount

The number of subdivisions in each face of the pyramid along its y-axis. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var heightSegmentCount: Int { get set }
```

## Discussion

A larger number of segments adds more vertex data to the geometry. Though each face of the pyramid is a flat plane, extra vertices can be useful for lighting or custom shader programs. Adding vertices increases rendering cost, so you should use the minimal segment count that produces your desired visual effect.

The default segment count is `1`. Setting this property’s value to a number less than `1` results in undefined behavior.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Adjusting Geometric Detail

var widthSegmentCount: Int

The number of subdivisions in each face of the pyramid along its x-axis. Animatable.

var lengthSegmentCount: Int

The number of subdivisions in each face of the pyramid along its z-axis. Animatable.

