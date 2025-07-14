

- RealityKit
- PointLightComponent
-  init(cgColor:intensity:attenuationRadius:) 

Initializer

# init(cgColor:intensity:attenuationRadius:)

Creates a new instance with the specified color, intensity and attenuation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS 2.0+

``` source
init(
    cgColor: CGColor,
    intensity: Float = 26963.76,
    attenuationRadius: Float = 10.0
)
```

## Parameters 

`cgColor`  

The color of the light.

`intensity`  

The light’s brightness.

`attenuationRadius`  

The distance from the light source where its intensity reaches zero. Any objects at or beyond this distance do not receive illumination.

## See Also

### Creating a point light component

init(color: PointLightComponent.Color, intensity: Float, attenuationRadius: Float)

Creates a point light component with a configuration.

init(color: PointLightComponent.Color, intensity: Float, attenuationRadius: Float)

Creates a point light component with a configuration.

init(color: PointLightComponent.Color, intensity: Float, attenuationRadius: Float, attenuationFalloffExponent: Float)

Creates a point light component with a configuration.

init(color: PointLightComponent.Color, intensity: Float, attenuationRadius: Float, attenuationFalloffExponent: Float)

Creates a point light component with a configuration.

