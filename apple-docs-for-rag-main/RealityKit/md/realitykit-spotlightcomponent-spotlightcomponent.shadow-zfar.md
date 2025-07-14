

- RealityKit
- SpotLightComponent
- SpotLightComponent.Shadow
-  zFar 

Instance Property

# zFar

The orthogonal plane of the shadow frustum that’s furthest from the spotlight.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var zFar: SpotLightComponent.Shadow.ShadowClippingPlane { get set }
```

## Discussion

The `zFar` is the maximum distance between the light and a visible surface for casting shadows.

The spotlight applies the value from attenuationRadius, when you set this property to SpotLightComponent.Shadow.ShadowClippingPlane.automatic, which is its default value. Setting this value to SpotLightComponent.Shadow.ShadowClippingPlane.fixed(_:) is equivalent to assigning it to `min(zFar, attenuationRadius)`.

## See Also

### Configuring the shadow

var depthBias: Float

A constant value that RealityKit applies as a bias to its shadow calculations.

var zNear: SpotLightComponent.Shadow.ShadowClippingPlane

The near-plane of a shadow frustum.

var cullModeOverride: SpotLightComponent.Shadow.ShadowMapCullMode?

The light’s culling mode for shadow map rendering.

