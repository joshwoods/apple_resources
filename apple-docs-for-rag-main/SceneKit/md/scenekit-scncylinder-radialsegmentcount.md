

- SceneKit
- SCNCylinder
-  radialSegmentCount 

Instance Property

# radialSegmentCount

The number of subdivisions around the circumference of the cylinder. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var radialSegmentCount: Int { get set }
```

## Discussion

A larger number of segments adds more vertex data to the geometry, creating a smoother curve for the cylinder’s circular cross section at a cost to rendering performance.

The default segment count is `48`. Setting this property’s value to a number less than `3` results in undefined behavior.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Adjusting Geometric Detail

var heightSegmentCount: Int

The number of subdivisions in the sides of the cylinder along its y-axis. Animatable.

