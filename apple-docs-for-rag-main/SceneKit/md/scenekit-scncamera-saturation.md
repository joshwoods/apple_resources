

- SceneKit
- SCNCamera
-  saturation 

Instance Property

# saturation

An adjustment factor to apply to the overall color saturation of the rendered scene.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var saturation: CGFloat { get set }
```

## Discussion

A value of `1.0` (the default) leaves scene colors unchanged. Greater values result in oversaturated colors, and a value of `0.0` makes the rendered scene entirely grayscale.

To enable this behavior, you must first enable the wantsHDR setting.

## See Also

### Adjusting Rendered Colors

var contrast: CGFloat

An adjustment factor to apply to the overall visual contrast of the rendered scene.

var colorGrading: SCNMaterialProperty

A texture for applying color grading effects to the entire rendered scene.

