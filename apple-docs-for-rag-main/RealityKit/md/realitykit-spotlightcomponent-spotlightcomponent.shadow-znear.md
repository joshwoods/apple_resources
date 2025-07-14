

- RealityKit
- SpotLightComponent
- SpotLightComponent.Shadow
-  zNear 

Instance Property

# zNear

The near-plane of a shadow frustum.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var zNear: SpotLightComponent.Shadow.ShadowClippingPlane { get set }
```

## Discussion

The `zNear` is the minimum distance between the light and a visible surface for casting shadows. The default value for `zNear` is SpotLightComponent.Shadow.ShadowClippingPlane.automatic.

## See Also

### Configuring the shadow

var depthBias: Float

A constant value that RealityKit applies as a bias to its shadow calculations.

var zFar: SpotLightComponent.Shadow.ShadowClippingPlane

The orthogonal plane of the shadow frustum that’s furthest from the spotlight.

var cullModeOverride: SpotLightComponent.Shadow.ShadowMapCullMode?

The light’s culling mode for shadow map rendering.

