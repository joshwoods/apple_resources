

- SceneKit
- SCNLight
-  orthographicScale 

Instance Property

# orthographicScale

The orthographic scale SceneKit uses when rendering the shadow map for a directional light.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var orthographicScale: CGFloat { get set }
```

## Discussion

SceneKit draws a shadow map image by rendering the scene from the point of view of the node containing the light. Directional lights ignore the position property of the node containing them because their light has a constant direction. Therefore, rendering a shadow map for a directional light requires an orthographic projection. Like the orthographicScale property of a camera object, this property specifies the extent of the scene “visible to” the light when rendering the shadow map.

This property applies only if the light’s type property is directional.

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

var zFar: CGFloat

The maximum distance between the light and a visible surface for casting shadows.

var zNear: CGFloat

The minimum distance between the light and a visible surface for casting shadows. Animatable.

