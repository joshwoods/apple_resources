

- RealityKit
- DirectionalLightComponent
- DirectionalLightComponent.Shadow
-  shadowProjection 

Instance Property

# shadowProjection

Sets the shadow projection used for shadow map rendering

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var shadowProjection: DirectionalLightComponent.Shadow.ShadowProjectionType { get set }
```

## See Also

### Configuring the shadow

var depthBias: Float

A constant value that RealityKit applies as a bias to its shadow calculations.

var cullModeOverride: DirectionalLightComponent.Shadow.ShadowMapCullMode?

The light’s culling mode for shadow map rendering.

var maximumDistance: Float

The maximum distance for the shadow.

Deprecated

