

- RealityKit
- DirectionalLightComponent
- DirectionalLightComponent.Shadow
-  init(maximumDistance:depthBias:) 

Initializer

# init(maximumDistance:depthBias:)

Creates a directional light shadow with a maximum distance and depth bias.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 2.0+

``` source
init(
    maximumDistance: Float = 5.0,
    depthBias: Float = 1.0
)
```

## Parameters 

`maximumDistance`  

The maximum distance for the shadow.

`depthBias`  

The depth bias for the shadow.

## Discussion

The `maximumDistance` parameter in this initializer is equivalent to setting shadowProjection to `.automatic(maximumDistance: maximumDistance)`.

## See Also

### Creating the shadow

init()

Creates a directional light shadow using default values.

init(shadowProjection: DirectionalLightComponent.Shadow.ShadowProjectionType, depthBias: Float, cullMode: DirectionalLightComponent.Shadow.ShadowMapCullMode?)

Creates a directional light shadow with a shadow projection, depth bias and cull mode.

