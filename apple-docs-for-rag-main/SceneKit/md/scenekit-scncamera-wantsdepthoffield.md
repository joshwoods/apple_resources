

- SceneKit
- SCNCamera
-  wantsDepthOfField 

Instance Property

# wantsDepthOfField

A Boolean value that determines whether SceneKit renders depth-of-field blur effects for the camera.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var wantsDepthOfField: Bool { get set }
```

## Discussion

This value is false by default, disabling depth-of-field effects.

Enabling this property causes SceneKit to render blur effects that model those created by a physical camera device (also known as *bokeh*). That is, objects in the scene appear more or less blurry depending on their distance from the camera and the camera’s focusDistance, and the intensity and style of the blur effect depend on the fStop and apertureBladeCount properties.

Note

For best results, also enable the wantsHDR property when using depth-of-field effects. High Dynamic Range rendering provides high contrast for distant bright points in the scene, creating more pronounced bokeh effects.

## See Also

### Adding Depth-of-Field Effects

var focusDistance: CGFloat

The distance from the camera at which objects appear in sharp focus. Animatable.

var fStop: CGFloat

The physical camera aperture simulated by SceneKit for depth-of-field effects. Animatable.

var apertureBladeCount: Int

The number of physical camera aperture blades simulated by SceneKit for depth-of-field effects.

var focalBlurSampleCount: Int

The number of pixel samples SceneKit uses to create depth-of-field blur effects.

