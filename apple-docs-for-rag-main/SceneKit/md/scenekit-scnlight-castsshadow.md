

- SceneKit
- SCNLight
-  castsShadow 

Instance Property

# castsShadow

A Boolean value that determines whether the light casts shadows.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var castsShadow: Bool { get set }
```

## Discussion

Geometries illuminated by the light cast shadows only if the value of this property is true and the type property of the light is spot or directional. The default value is false.

## See Also

### Managing Shadows Cast by the Light

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

var zNear: CGFloat

The minimum distance between the light and a visible surface for casting shadows. Animatable.

