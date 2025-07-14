

- SceneKit
- SCNTorus
-  ringSegmentCount 

Instance Property

# ringSegmentCount

The number of subdivisions around the torus ring. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var ringSegmentCount: Int { get set }
```

## Discussion

This segment count corresponds to the circle formed by the torus’ major radius or ringRadius property. A larger number of segments adds more vertex data to the geometry, creating a more smoothly curved surface at a cost to rendering performance.

The default segment count is `48`. Setting this property’s value to a number less than `3` results in undefined behavior.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Configuring Torus Properties

var pipeSegmentCount: Int

The number of subdivisions around the torus pipe. Animatable.

