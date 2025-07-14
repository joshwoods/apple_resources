

- SceneKit
- SCNCamera
-  focalBlurSampleCount 

Instance Property

# focalBlurSampleCount

The number of pixel samples SceneKit uses to create depth-of-field blur effects.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var focalBlurSampleCount: Int { get set }
```

## Discussion

When the wantsDepthOfField setting is enabled, SceneKit renders depth-of-field blur (also called *bokeh*) effects using a blur filter that samples multiple points in the image. Sampling a larger number of points produces a higher quality visual effect at a higher performance cost, and vice versa. The default sample count is 25.

## See Also

### Adding Depth-of-Field Effects

var wantsDepthOfField: Bool

A Boolean value that determines whether SceneKit renders depth-of-field blur effects for the camera.

var focusDistance: CGFloat

The distance from the camera at which objects appear in sharp focus. Animatable.

var fStop: CGFloat

The physical camera aperture simulated by SceneKit for depth-of-field effects. Animatable.

var apertureBladeCount: Int

The number of physical camera aperture blades simulated by SceneKit for depth-of-field effects.

