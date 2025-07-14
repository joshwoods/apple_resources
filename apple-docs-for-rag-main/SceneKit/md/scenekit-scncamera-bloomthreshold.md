

- SceneKit
- SCNCamera
-  bloomThreshold 

Instance Property

# bloomThreshold

The brightness threshold at which to apply a bloom effect to highlights in the rendered scene. Animatable.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var bloomThreshold: CGFloat { get set }
```

## Discussion

A bloom effect adds a soft glow to highlights (areas of bright color) in the rendered scene, simulating the way bright highlights appear to the human eye or a physical camera in a real-world scene. This property controls the brightness level required to trigger the bloom effect; lower values apply the effect to more of the scene, and higher values apply the effect only to the brightest white areas. The default value is `1.0`.

You can animate changes to this property’s value. See Animating SceneKit Content.

To enable this behavior, you must first enable the wantsHDR setting.

## See Also

### Adding Stylistic Visual Effects

var bloomIntensity: CGFloat

The magnitude of bloom effect to apply to highlights in the rendered scene. Animatable.

var bloomBlurRadius: CGFloat

The radius, in pixels, for the blurring portion of the bloom effect applied to highlights in the rendered scene. Animatable.

var colorFringeIntensity: CGFloat

The blend factor for fading the color fringing effect applied to the rendered scene.

var colorFringeStrength: CGFloat

The magnitude of color fringing effect to apply to the rendered scene.

var vignettingIntensity: CGFloat

The magnitude of vignette (darkening around edges) effect to apply to the rendered scene.

var vignettingPower: CGFloat

The amount of the rendered scene to darken with a vignette effect.

