

- SceneKit
- SCNLight
-  shadowBias 

Instance Property

# shadowBias

The amount of correction to apply to the shadow to prevent rendering artifacts.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var shadowBias: CGFloat { get set }
```

## Discussion

Rendering shadows from a shadow map can result in artifacts where the shadow color does not appear on all pixels in a shadowed surface as intended. (This effect is typically called *shadow acne*.) This property specifies the error margin SceneKit uses to correct such artifacts.

The default value is `1.0`.

## See Also

### Managing Shadows Cast by the Light

var castsShadow: Bool

A Boolean value that determines whether the light casts shadows.

var shadowRadius: CGFloat

A number that specifies the amount of blurring around the edges of shadows cast by the light. Animatable.

var shadowColor: Any

The color of shadows cast by the light. Animatable.

var shadowMapSize: CGSize

The size of the shadow map image that SceneKit renders when creating shadows.

var shadowSampleCount: Int

The number of samples from the shadow map that SceneKit uses to render each pixel.

var shadowMode: SCNShadowMode

The mode SceneKit uses to render shadows.

enum SCNShadowMode

Options for SceneKit’s rendering of shadows cast by a light, used by the shadowMode property.

var orthographicScale: CGFloat

The orthographic scale SceneKit uses when rendering the shadow map for a directional light.

var zFar: CGFloat

The maximum distance between the light and a visible surface for casting shadows.

var zNear: CGFloat

The minimum distance between the light and a visible surface for casting shadows. Animatable.

