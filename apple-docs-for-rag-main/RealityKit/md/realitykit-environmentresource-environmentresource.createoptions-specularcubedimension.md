

- RealityKit
- EnvironmentResource
- EnvironmentResource.CreateOptions
-  specularCubeDimension 

Instance Property

# specularCubeDimension

The dimension of the computed specular cubemap for material reflections.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var specularCubeDimension: Int?
```

## Discussion

If `nil`, the environment resource uses the source cubemap’s dimensions.

A value lower than that of the cubemap helps to reduce the memory footprint in scenes where you view skybox details through specular reflections.

Note

The specular cube dimension clamps to the source cubemap’s dimensions if it exceeds them.

## See Also

### Accessing the option properties

var compression: EnvironmentResource.Compression

The compression to apply to environment textures.

var samplingQuality: EnvironmentResource.CreateOptions.SamplingQuality

The skybox sampling quality for lighting textures.

