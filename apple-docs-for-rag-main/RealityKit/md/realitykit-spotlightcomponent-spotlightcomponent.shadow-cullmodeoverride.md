

- RealityKit
- SpotLightComponent
- SpotLightComponent.Shadow
-  cullModeOverride 

Instance Property

# cullModeOverride

The light’s culling mode for shadow map rendering.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var cullModeOverride: SpotLightComponent.Shadow.ShadowMapCullMode? { get set }
```

## See Also

### Configuring the shadow

var depthBias: Float

A constant value that RealityKit applies as a bias to its shadow calculations.

var zNear: SpotLightComponent.Shadow.ShadowClippingPlane

The near-plane of a shadow frustum.

var zFar: SpotLightComponent.Shadow.ShadowClippingPlane

The orthogonal plane of the shadow frustum that’s furthest from the spotlight.

