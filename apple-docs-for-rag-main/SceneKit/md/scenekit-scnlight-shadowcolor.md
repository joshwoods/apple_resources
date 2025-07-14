

- SceneKit
- SCNLight
-  shadowColor 

Instance Property

# shadowColor

The color of shadows cast by the light. Animatable.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var shadowColor: Any { get set }
```

## Discussion

The value of this property is an NSColor or CGColor object. SceneKit blends the light’s color with other colors in the rendered image to produce a shadow effect. The color’s opacity (alpha value) determines the intensity of the shadows. The default shadow color is black with 50% opacity.

You can animate changes to this property’s value. See Animating SceneKit Content.

## See Also

### Managing Shadows Cast by the Light

var castsShadow: Bool

A Boolean value that determines whether the light casts shadows.

var shadowRadius: CGFloat

A number that specifies the amount of blurring around the edges of shadows cast by the light. Animatable.

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

