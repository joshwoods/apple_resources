

- SceneKit
- SCNCamera
-  vignettingIntensity 

Instance Property

# vignettingIntensity

The magnitude of vignette (darkening around edges) effect to apply to the rendered scene.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var vignettingIntensity: CGFloat { get set }
```

## Discussion

A vignette effect darkens the edges and corners of the rendered scene, simulating the effect of lens and barrel shape on the image produced by a physical camera. Higher values result in more darkening, and lower values result in a subtler effect. The default value of `0.0` results in no vignetting effect.

This property controls the level of darkening applied; the vignettingPower property controls the area of the rendered image to be darkened.

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

var colorFringeStrength: CGFloat

The magnitude of color fringing effect to apply to the rendered scene.

var vignettingPower: CGFloat

The amount of the rendered scene to darken with a vignette effect.

