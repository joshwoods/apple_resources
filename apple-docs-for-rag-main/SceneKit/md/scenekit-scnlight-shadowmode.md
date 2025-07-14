

- SceneKit
- SCNLight
-  shadowMode 

Instance Property

# shadowMode

The mode SceneKit uses to render shadows.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var shadowMode: SCNShadowMode { get set }
```

## Discussion

The default mode is SCNShadowMode.forward in iOS and in macOS 10.10 or later. In OS X v10.9 or earlier, the default mode is SCNShadowMode.deferred.

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

