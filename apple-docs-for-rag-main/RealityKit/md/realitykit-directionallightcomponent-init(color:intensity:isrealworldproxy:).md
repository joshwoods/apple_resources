

- RealityKit
- DirectionalLightComponent
-  init(color:intensity:isRealWorldProxy:) 

Initializer

# init(color:intensity:isRealWorldProxy:)

Creates a directional light with a configuration.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+

``` source
init(
    color: DirectionalLightComponent.Color = .white,
    intensity: Float = 2145.7078,
    isRealWorldProxy: Bool = false
)
```

## Parameters 

`color`  

A color for the light.

`intensity`  

The intensity of the light, measured in lumen per square meter.

`isRealWorldProxy`  

A Boolean that you use to control whether the light operates as a proxy for a real-world light.

## See Also

### Creating a directional light

init(color: DirectionalLightComponent.Color, intensity: Float)

Creates a directional light with a configuration.

init(color: DirectionalLightComponent.Color, intensity: Float, isRealWorldProxy: Bool)

Creates a directional light with a configuration.

