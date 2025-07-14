

- SceneKit
- SCNTorus
-  pipeSegmentCount 

Instance Property

# pipeSegmentCount

The number of subdivisions around the torus pipe. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var pipeSegmentCount: Int { get set }
```

## Discussion

This segment count corresponds to the circle formed by the torus’ minor radius or pipeRadius property. A larger number of segments adds more vertex data to the geometry, creating a more smoothly curved surface at a cost to rendering performance.

The default segment count is `24`. Setting this property’s value to a number less than `3` results in undefined behavior.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Configuring Torus Properties

var ringSegmentCount: Int

The number of subdivisions around the torus ring. Animatable.

