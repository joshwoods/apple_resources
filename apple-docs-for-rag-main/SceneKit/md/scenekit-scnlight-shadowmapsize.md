

- SceneKit
- SCNLight
-  shadowMapSize 

Instance Property

# shadowMapSize

The size of the shadow map image that SceneKit renders when creating shadows.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var shadowMapSize: CGSize { get set }
```

## Discussion

SceneKit produces shadows by rendering the silhouettes of scene geometry into a 2D shadow map image and then projecting that image into the rendered scene. A larger shadow map image produces more detailed shadows at a higher cost to rendering performance; a smaller shadow map renders more quickly but results in pixelation at the edges of shadows.

The default value is CGSizeZero, specifying that SceneKit chooses a shadow map size automatically.

## See Also

### Managing Shadows Cast by the Light

var castsShadow: Bool

A Boolean value that determines whether the light casts shadows.

var shadowRadius: CGFloat

A number that specifies the amount of blurring around the edges of shadows cast by the light. Animatable.

var shadowColor: Any

The color of shadows cast by the light. Animatable.

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

