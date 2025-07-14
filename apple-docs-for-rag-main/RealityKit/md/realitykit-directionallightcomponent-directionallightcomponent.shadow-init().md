

- RealityKit
- DirectionalLightComponent
- DirectionalLightComponent.Shadow
-  init() 

Initializer

# init()

Creates a directional light shadow using default values.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 2.0+

``` source
init()
```

## See Also

### Creating the shadow

init(shadowProjection: DirectionalLightComponent.Shadow.ShadowProjectionType, depthBias: Float, cullMode: DirectionalLightComponent.Shadow.ShadowMapCullMode?)

Creates a directional light shadow with a shadow projection, depth bias and cull mode.

init(maximumDistance: Float, depthBias: Float)

Creates a directional light shadow with a maximum distance and depth bias.

