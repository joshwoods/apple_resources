

- SceneKit
- SCNCamera
-  zFar 

Instance Property

# zFar

The camera’s far depth limit. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var zFar: Double { get set }
```

## Discussion

The far value determines the maximal distance between the camera and a visible surface. If a surface is farther from the camera than this distance, the surface is clipped and does not appear. The default far value is `100.0`.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Adjusting Camera Perspective

var zNear: Double

The camera’s near depth limit. Animatable.

var automaticallyAdjustsZRange: Bool

A Boolean value that determines whether the camera automatically adjusts its zNear and zFar depth limits.

