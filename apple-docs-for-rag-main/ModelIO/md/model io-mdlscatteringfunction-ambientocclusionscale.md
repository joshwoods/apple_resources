

- Model I/O
- MDLScatteringFunction
-  ambientOcclusionScale 

Instance Property

# ambientOcclusionScale

The scaling factor for ambient occlusion shading.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var ambientOcclusionScale: MDLMaterialProperty { get }
```

## Discussion

The default scaling factor is `1.0`. Modify this value to increase or decrease the severity of ambient occlusion shading.

## See Also

### Working with Shading Properties

var baseColor: MDLMaterialProperty

The inherent color of the material, to be used as a modulator during shading.

var emission: MDLMaterialProperty

The color emitted as radiance from a material’s surface.

var specular: MDLMaterialProperty

The intensity of specular highlights on the material’s surface.

var materialIndexOfRefraction: MDLMaterialProperty

The index of refraction for the medium surrounding a material.

var interfaceIndexOfRefraction: MDLMaterialProperty

The index of refraction for a material itself.

var normal: MDLMaterialProperty

The variation in the surface normal vectors in a material, relative to model coordinate space.

var ambientOcclusion: MDLMaterialProperty

The attenuation of ambient light due to local geometry variations on a surface.

