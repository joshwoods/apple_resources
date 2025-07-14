

- RealityKit
- CustomMaterial
-  ambientOcclusion 

Instance Property

# ambientOcclusion

The ambient light exposure for a material.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var ambientOcclusion: CustomMaterial.AmbientOcclusion { get set }
```

## Discussion

Ambient occlusion (AO) represents the entity’s exposure to ambient light. Specify ambient occlusion using a UV-mapped image called an *ambient occlusion map*. In an AO map, black pixels represent parts of the model that receive no ambient light because of a crevice, dent, or recessed area, or another part of the entity blocking ambient light from reaching it. White pixels represent flat portions of the model that receive full ambient light. You generate ambient occlusion maps using a 3D software package.

The following code loads an ambient occlusion map and adds it to the custom material:

```
if let aoResource = try? TextureResource.load(named:"entity_ao") {
    let aoMap = MaterialParameters.Texture(aoResource)
    material.emissiveColor = .init(texture: aoMap)
}
```

In a custom material, RealityKit doesn’t automatically use the value you set on this property to render your entity. The ambient occlusion texture is available in the material’s shader functions, but RealityKit only renders ambient occlusion if the material’s lightingModel is CustomMaterial.LightingModel.lit or CustomMaterial.LightingModel.clearcoat and its surface shader calls `params.surface().set_ambient_occlusion()`.

The following Metal code shows how to sample the ambient occlusion texture to set the AO value in a surface shader function:

```
// Retrieve the entity's texture coordinates.
float2 uv = params.geometry().uv0();

// Entities loaded from USDZ or .reality files have texture coordinates
// with a flipped y-axis. This adjusts for that.
uv.y = 1.0 - uv.y;

// Sample the ambient occlusion texture and use it to set the
// ambient occlusion value to use during rendering.
auto tex = params.textures();
half metallic = tex.ambient_occlusion().sample(textureSampler, uv).r;
params.surface().set_ambient_occlusion(metallic);
```

## See Also

### Setting the core properties

var baseColor: CustomMaterial.BaseColor

The color of an entity unmodified by lighting.

var roughness: CustomMaterial.Roughness

The amount the surface of the 3D object scatters reflected light.

var metallic: CustomMaterial.Metallic

The reflectiveness of an entity.

var normal: CustomMaterial.Normal

A texture map that stores fine surface details for the entity.

var emissiveColor: CustomMaterial.EmissiveColor

The color of light this material emits.

var specular: CustomMaterial.Specular

The bright highlights to apply to the entity.

var clearcoat: CustomMaterial.Clearcoat

The transparent highlights that simulate a clear, shiny coating on an entity.

var clearcoatRoughness: CustomMaterial.ClearcoatRoughness

The degree to which an entity’s clear, shiny coating scatters light to create soft highlights.

var clearcoatNormal: CustomMaterial.ClearcoatNormal

Waviness and imperfections for the top clearcoat.

