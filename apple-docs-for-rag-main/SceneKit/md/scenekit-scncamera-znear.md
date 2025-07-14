

- SceneKit
- SCNCamera
-  zNear 

Instance Property

# zNear

The camera’s near depth limit. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var zNear: Double { get set }
```

## Discussion

The near value determines the minimal distance between the camera and a visible surface. If a surface is closer to the camera than this distance, the surface is clipped and does not appear. The near value must not be zero. The default near value is `1.0`.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Adjusting Camera Perspective

var zFar: Double

The camera’s far depth limit. Animatable.

var automaticallyAdjustsZRange: Bool

A Boolean value that determines whether the camera automatically adjusts its zNear and zFar depth limits.

