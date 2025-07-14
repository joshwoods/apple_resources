

- SceneKit
- SCNCamera
-  wantsHDR 

Instance Property

# wantsHDR

A Boolean value that determines whether SceneKit applies High Dynamic Range (HDR) postprocessing effects to a scene.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var wantsHDR: Bool { get set }
```

## Discussion

When this property’s value is false (the default), SceneKit performs lighting calculations in a color space whose brightness range is similar to that of the output display. This approach limits the ability to perform realistic rendering of scenes with fine details in brightness levels.

When you enable HDR rendering for a camera, SceneKit calculates lighting in a much deeper color space, preserving fine details in contrast regardless of brightness, then applies a post-processing effect called *tone mapping* to translate luminance values from that space to the narrower range of brightness values that can be shown on a display. SceneKit determines a tone mapping curve (including the exposure level) from the minimumExposure, maximumExposure, exposureOffset, and whitePoint properties along with a measure of scene luminance. The wantsExposureAdaptation property determines whether tone mapping effects are static or dynamically respond when the luminance visible to the camera changes.

The default value is false.

## See Also

### Adding High Dynamic Range Effects

var exposureOffset: CGFloat

A logarithmic bias that adjusts the results of SceneKit’s tone mapping operation, brightening or darkening the visible scene.

var averageGray: CGFloat

The luminance level to use as the midpoint of a tone mapping curve.

var whitePoint: CGFloat

The luminance level to use as the upper end of a tone mapping curve.

var minimumExposure: CGFloat

The minimum exposure value to use in tone mapping.

var maximumExposure: CGFloat

The minimum exposure value to use in tone mapping.

