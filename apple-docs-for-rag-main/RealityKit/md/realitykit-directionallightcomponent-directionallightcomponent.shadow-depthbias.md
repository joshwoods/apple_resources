

- RealityKit
- DirectionalLightComponent
- DirectionalLightComponent.Shadow
-  depthBias 

Instance Property

# depthBias

A constant value that RealityKit applies as a bias to its shadow calculations.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 2.0+

``` source
var depthBias: Float
```

## Discussion

Reduce visual effects such as *shadow acne*, by adjusting this property. The default value is `1.0`.

## See Also

### Configuring the shadow

var cullModeOverride: DirectionalLightComponent.Shadow.ShadowMapCullMode?

The light’s culling mode for shadow map rendering.

var shadowProjection: DirectionalLightComponent.Shadow.ShadowProjectionType

Sets the shadow projection used for shadow map rendering

var maximumDistance: Float

The maximum distance for the shadow.

Deprecated

