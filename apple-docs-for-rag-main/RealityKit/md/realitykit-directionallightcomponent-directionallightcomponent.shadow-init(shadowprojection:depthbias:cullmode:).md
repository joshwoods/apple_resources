

- RealityKit
- DirectionalLightComponent
- DirectionalLightComponent.Shadow
-  init(shadowProjection:depthBias:cullMode:) 

Initializer

# init(shadowProjection:depthBias:cullMode:)

Creates a directional light shadow with a shadow projection, depth bias and cull mode.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    shadowProjection: DirectionalLightComponent.Shadow.ShadowProjectionType,
    depthBias: Float,
    cullMode: DirectionalLightComponent.Shadow.ShadowMapCullMode? = nil
)
```

## Parameters 

`shadowProjection`  

The shadow projection used for shadow map rendering.

`depthBias`  

The depth bias for the shadow.

`cullMode`  

The mode used to cull faces when generating the shadow.

## See Also

### Creating the shadow

init()

Creates a directional light shadow using default values.

init(maximumDistance: Float, depthBias: Float)

Creates a directional light shadow with a maximum distance and depth bias.

