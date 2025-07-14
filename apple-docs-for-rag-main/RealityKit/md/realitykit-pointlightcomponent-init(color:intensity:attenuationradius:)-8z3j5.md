

- RealityKit
- PointLightComponent
-  init(color:intensity:attenuationRadius:) 

Initializer

# init(color:intensity:attenuationRadius:)

Creates a point light component with a configuration.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 2.0+

``` source
init(
    color: PointLightComponent.Color = .white,
    intensity: Float = 26963.76,
    attenuationRadius: Float = 10.0
)
```

## Parameters 

`color`  

The color of the light.

`intensity`  

The intensity of the light in lumens.

`attenuationRadius`  

The distance from the light source where its intensity reaches zero. Any objects at or beyond this distance do not receive illumination.

## See Also

### Creating a point light component

init(color: PointLightComponent.Color, intensity: Float, attenuationRadius: Float)

Creates a point light component with a configuration.

init(cgColor: CGColor, intensity: Float, attenuationRadius: Float)

Creates a new instance with the specified color, intensity and attenuation.

init(color: PointLightComponent.Color, intensity: Float, attenuationRadius: Float, attenuationFalloffExponent: Float)

Creates a point light component with a configuration.

init(color: PointLightComponent.Color, intensity: Float, attenuationRadius: Float, attenuationFalloffExponent: Float)

Creates a point light component with a configuration.

