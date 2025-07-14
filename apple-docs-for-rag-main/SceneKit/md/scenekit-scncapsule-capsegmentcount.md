

- SceneKit
- SCNCapsule
-  capSegmentCount 

Instance Property

# capSegmentCount

The number of subdivisions in the height of each hemispherical end of the capsule. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var capSegmentCount: Int { get set }
```

## Discussion

A larger number of segments adds more vertex data to the geometry, creating a smoother curved surface for the capsule’s ends at a cost to rendering performance.

The default segment count is `24`. Setting this property’s value to a number less than `1` results in undefined behavior.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Adjusting Geometric Detail

var radialSegmentCount: Int

The number of subdivisions around the lateral circumference of the capsule. Animatable.

var heightSegmentCount: Int

The number of subdivisions in the sides of the capsule along its y-axis. Animatable.

