

- SceneKit
- SCNCamera
-  fStop 

Instance Property

# fStop

The physical camera aperture simulated by SceneKit for depth-of-field effects. Animatable.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var fStop: CGFloat { get set }
```

## Discussion

F-stop numbers describe the light-gathering area of a physical camera’s imaging system, and are typically expressed as the denominator of a ratio including the camera’s focal length ƒ, such as ƒ/2 or ƒ/5.6. A larger denominator indicates a smaller aperture, allowing less light to pass from the camera’s lens through to the imaging plane (sensor or film), and a smaller denominator indicates a larger aperture that lets more light through.

SceneKit uses aperture measurements to simulate depth-of-field blur effects (also called *bokeh*) approximating those produced by a physical camera. A larger fStop number (or aperture denominator) causes most of the scene to appear in focus, with extremely close or far depths showing slight blurring; a smaller number results in only a narrow range of depths appearing in focus, and a more pronounced blur effect for the rest of the scene. The default fStop value is `5.6`.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Adding Depth-of-Field Effects

var wantsDepthOfField: Bool

A Boolean value that determines whether SceneKit renders depth-of-field blur effects for the camera.

var focusDistance: CGFloat

The distance from the camera at which objects appear in sharp focus. Animatable.

var apertureBladeCount: Int

The number of physical camera aperture blades simulated by SceneKit for depth-of-field effects.

var focalBlurSampleCount: Int

The number of pixel samples SceneKit uses to create depth-of-field blur effects.

