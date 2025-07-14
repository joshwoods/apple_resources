

- RealityKit
- EnvironmentResource
- EnvironmentResource.CreateOptions
-  init(samplingQuality:specularCubeDimension:compression:) 

Initializer

# init(samplingQuality:specularCubeDimension:compression:)

Creates an environment creation options structure.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    samplingQuality: EnvironmentResource.CreateOptions.SamplingQuality = .fast,
    specularCubeDimension: Int? = nil,
    compression: EnvironmentResource.Compression = .default
)
```

## Parameters 

`samplingQuality`  

The skybox sampling quality for lighting textures.

`specularCubeDimension`  

The dimension of the computed specular cubemap for material reflections.

`compression`  

The compression to apply to environment textures.

