

- SceneKit
- SCNCamera
-  colorFringeStrength 

Instance Property

# colorFringeStrength

The magnitude of color fringing effect to apply to the rendered scene.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var colorFringeStrength: CGFloat { get set }
```

## Discussion

Color fringing applies an effect that separately blurs the color components of each rendered pixel, adding subtle rainbow edge effects to the rendered scene that simulate the effects of chromatic aberration in a physical camera. Higher values create a more pronounced color shift, creating wider rainbow fringes; lower values spread colors across shorter distances, creating a subtler effect. The default value of `0.0` disables the color fringing effect entirely.

This property controls the breadth of color fringing. The colorFringeIntensity property controls the blend factor between the color-fringed and the otherwise-normally-rendered image.

To enable this behavior, you must first enable the wantsHDR setting.

## See Also

### Adding Stylistic Visual Effects

var bloomIntensity: CGFloat

The magnitude of bloom effect to apply to highlights in the rendered scene. Animatable.

var bloomThreshold: CGFloat

The brightness threshold at which to apply a bloom effect to highlights in the rendered scene. Animatable.

var bloomBlurRadius: CGFloat

The radius, in pixels, for the blurring portion of the bloom effect applied to highlights in the rendered scene. Animatable.

var colorFringeIntensity: CGFloat

The blend factor for fading the color fringing effect applied to the rendered scene.

var vignettingIntensity: CGFloat

The magnitude of vignette (darkening around edges) effect to apply to the rendered scene.

var vignettingPower: CGFloat

The amount of the rendered scene to darken with a vignette effect.

