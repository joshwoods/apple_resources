

- Model I/O
- MDLScatteringFunction
-  ambientOcclusion 

Instance Property

# ambientOcclusion

The attenuation of ambient light due to local geometry variations on a surface.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var ambientOcclusion: MDLMaterialProperty { get }
```

## Discussion

Ambient occlusion (AO) describes the accessibility of a point on a surface to the surrounding radiant environment and is typically used to attenuate ambient lighting. A renderer should not use AO data should to affect direct illumination.

The default AO value is zero. Typically, you assign a texture (such as that created with the generateAmbientOcclusionTexture(withQuality:attenuationFactor:objectsToConsider:vertexAttributeNamed:materialPropertyNamed:) method of a mesh) to this material property to add shading based on the shape of the mesh.

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

var ambientOcclusionScale: MDLMaterialProperty

The scaling factor for ambient occlusion shading.

