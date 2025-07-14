

- SceneKit
- SCNCapsule
-  heightSegmentCount 

Instance Property

# heightSegmentCount

The number of subdivisions in the sides of the capsule along its y-axis. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var heightSegmentCount: Int { get set }
```

## Discussion

A larger number of segments adds more vertex data to the geometry. Although the sides of the capsule’s cylindrical body are flat in the y-axis direction, extra vertices can be useful for lighting or custom shader programs. Adding vertices increases rendering cost, so use the minimal segment count that produces your desired visual effect.

The default segment count is `1`. Setting this property’s value to a number less than `1` results in undefined behavior.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Adjusting Geometric Detail

var radialSegmentCount: Int

The number of subdivisions around the lateral circumference of the capsule. Animatable.

var capSegmentCount: Int

The number of subdivisions in the height of each hemispherical end of the capsule. Animatable.

