

- Model I/O
- MDLScatteringFunction
-  baseColor 

Instance Property

# baseColor

The inherent color of the material, to be used as a modulator during shading.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var baseColor: MDLMaterialProperty { get }
```

## Discussion

The default base color is medium gray (50% white).

## See Also

### Working with Shading Properties

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

var ambientOcclusionScale: MDLMaterialProperty

The scaling factor for ambient occlusion shading.

