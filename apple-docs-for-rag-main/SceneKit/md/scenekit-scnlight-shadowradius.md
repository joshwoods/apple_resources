

- SceneKit
- SCNLight
-  shadowRadius 

Instance Property

# shadowRadius

A number that specifies the amount of blurring around the edges of shadows cast by the light. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var shadowRadius: CGFloat { get set }
```

## Discussion

SceneKit produces soft-edged shadows by rendering the silhouettes of geometry into a 2D shadow map and then using several weighted samples from the shadow map to determine the strength of the shadow at each pixel in the rendered scene. This property controls the radius of shadow map sampling. Lower numbers result in shadows with sharply defined, pixelated edges; higher numbers result in blurry shadows.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Managing Shadows Cast by the Light

var castsShadow: Bool

A Boolean value that determines whether the light casts shadows.

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

