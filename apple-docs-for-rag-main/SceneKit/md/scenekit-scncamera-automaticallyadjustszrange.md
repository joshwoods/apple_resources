

- SceneKit
- SCNCamera
-  automaticallyAdjustsZRange 

Instance Property

# automaticallyAdjustsZRange

A Boolean value that determines whether the camera automatically adjusts its zNear and zFar depth limits.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
var automaticallyAdjustsZRange: Bool { get set }
```

## Discussion

The default value of this property is false, specifying that the camera’s zNear and zFar properties control its depth limits. If you change this property’s value to true, SceneKit automatically adjusts the depth limits at render time to fit the bounding box of the scene. Changing the values of the zNear and zFar properties automatically resets this property’s value to false.

## See Also

### Adjusting Camera Perspective

var zNear: Double

The camera’s near depth limit. Animatable.

var zFar: Double

The camera’s far depth limit. Animatable.

