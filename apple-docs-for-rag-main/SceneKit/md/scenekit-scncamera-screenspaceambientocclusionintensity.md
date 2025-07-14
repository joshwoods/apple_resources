

- SceneKit
- SCNCamera
-  screenSpaceAmbientOcclusionIntensity 

Instance Property

# screenSpaceAmbientOcclusionIntensity

The intensity of the screen-space ambient occlusion effect applied in camera rendering.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var screenSpaceAmbientOcclusionIntensity: CGFloat { get set }
```

## Discussion

Ambient occlusion is an effect that improves material shading by calculating the amounts of ambient light that reach various parts of a surface, creating shadows on parts of a geometry where incoming light is obscured by other parts of the geometry. (You can provide pre-rendered ambient occlusion effects for a material using its ambientOcclusion property.) *Screen-space ambient occlusion* (SSAO) provides a real-time approximation of this effect for the entire scene viewed through the camera.

The default value of this property is zero, disabling SSAO effects. Increasing the intensity value creates deeper, bolder shadows.

## See Also

### Adding Screen-Space Ambient Occlusion

var screenSpaceAmbientOcclusionRadius: CGFloat

The distance, in units of scene space, at which ambient occlusion takes effect.

var screenSpaceAmbientOcclusionBias: CGFloat

An offset for modulating ambient occlusion effects.

var screenSpaceAmbientOcclusionDepthThreshold: CGFloat

The maximum depth difference, in units of scene space, at which to apply ambient occlusion effects.

var screenSpaceAmbientOcclusionNormalThreshold: CGFloat

The magnitude of the blur effect applied to create ambient occlusion shadows.

