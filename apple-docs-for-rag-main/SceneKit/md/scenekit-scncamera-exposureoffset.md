

- SceneKit
- SCNCamera
-  exposureOffset 

Instance Property

# exposureOffset

A logarithmic bias that adjusts the results of SceneKit’s tone mapping operation, brightening or darkening the visible scene.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var exposureOffset: CGFloat { get set }
```

## Discussion

When using a High Dynamic Range (HDR) camera, SceneKit applies a process called *tone mapping* to translate the wide range of luminance values in the visible scene to the narrower range of brightness values that can be shown on a display. SceneKit determines a tone mapping curve from the minimumExposure, maximumExposure, exposureOffset, and whitePoint properties, along with a measure of scene luminance.

Use this property to bias the tone mapping curve. The default exposure offset is zero, specifying no bias. Positive values result in a brighter scene, and negative values result in a darker scene.

This property has no effect if the wantsHDR value is false.

## See Also

### Adding High Dynamic Range Effects

var wantsHDR: Bool

A Boolean value that determines whether SceneKit applies High Dynamic Range (HDR) postprocessing effects to a scene.

var averageGray: CGFloat

The luminance level to use as the midpoint of a tone mapping curve.

var whitePoint: CGFloat

The luminance level to use as the upper end of a tone mapping curve.

var minimumExposure: CGFloat

The minimum exposure value to use in tone mapping.

var maximumExposure: CGFloat

The minimum exposure value to use in tone mapping.

