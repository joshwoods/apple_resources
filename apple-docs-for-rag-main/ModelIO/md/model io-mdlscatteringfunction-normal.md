

- Model I/O
- MDLScatteringFunction
-  normal 

Instance Property

# normal

The variation in the surface normal vectors in a material, relative to model coordinate space.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var normal: MDLMaterialProperty { get }
```

## Discussion

The default normal value is zero (no variation in surface normal vectors). Typically, you assign a texture to this material property to create the appearance of detailed surface contours.

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

var ambientOcclusion: MDLMaterialProperty

The attenuation of ambient light due to local geometry variations on a surface.

var ambientOcclusionScale: MDLMaterialProperty

The scaling factor for ambient occlusion shading.

