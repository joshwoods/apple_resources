

- SceneKit
- SCNLight
-  zNear 

Instance Property

# zNear

The minimum distance between the light and a visible surface for casting shadows. Animatable.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var zNear: CGFloat { get set }
```

## Discussion

A spotlight casts shadows if its castsShadow property is true. If a surface is closer to the light than this distance, shadows are not cast against the surface.

The default value is `1.0`.

You can animate changes to this property’s value. See Animating SceneKit Content.

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

var shadowBias: CGFloat

The amount of correction to apply to the shadow to prevent rendering artifacts.

var orthographicScale: CGFloat

The orthographic scale SceneKit uses when rendering the shadow map for a directional light.

var zFar: CGFloat

The maximum distance between the light and a visible surface for casting shadows.

