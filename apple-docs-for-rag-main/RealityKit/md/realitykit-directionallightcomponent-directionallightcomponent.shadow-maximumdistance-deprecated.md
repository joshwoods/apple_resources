

- RealityKit
- DirectionalLightComponent
- DirectionalLightComponent.Shadow
-  maximumDistance Deprecated

Instance Property

# maximumDistance

The maximum distance for the shadow.

iOS 13.0–18.0DeprecatediPadOS 13.0–18.0DeprecatedMac Catalyst 13.0–18.0DeprecatedmacOS 10.15–15.0Deprecated

``` source
var maximumDistance: Float { get set }
```

Deprecated

Use .shadowProjection = .automatic(maximumDistance:)

## See Also

### Configuring the shadow

var depthBias: Float

A constant value that RealityKit applies as a bias to its shadow calculations.

var cullModeOverride: DirectionalLightComponent.Shadow.ShadowMapCullMode?

The light’s culling mode for shadow map rendering.

var shadowProjection: DirectionalLightComponent.Shadow.ShadowProjectionType

Sets the shadow projection used for shadow map rendering

