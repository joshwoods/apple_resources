

- RealityKit
- CustomMaterial
-  specular 

Instance Property

# specular

The bright highlights to apply to the entity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var specular: CustomMaterial.Specular { get set }
```

## Discussion

In physically based rendering (PBR), specular highlights primarily come from the object’s roughness value. RealityKit renders materials that have a low roughness value with specular highlights based on the environment, lighting, and shape of the entity. As a result, for most materials, you don’t need to specify a `specular` value.

For some types of dielectric (nonmetallic) materials, like facet-cut glass or gems, PBR algorithms don’t create bright enough specular highlights using just roughness. To accurately simulate those types of materials, the specular property allows you to specify additional specularity for the entity.

The following example demonstrates how to add specularity using a single value for the entire material:

```
material.specular = .init(floatLiteral: 0.8)
```

The following code shows how to add specularity using a UV-mapped image texture:

```
if let specularResource = try? TextureResource.load(named: "entity_specular") {
    let specularMap = MaterialParameters.Texture(specularResource)
    material.specular = .init(texture: specularMap)
}
```

With custom materials, the specular scale and texture are available to the material’s shader functions, but RealityKit doesn’t automatically use the values you set. To render a custom material with additional specular highlights, set lightingModel to CustomMaterial.LightingModel.lit or CustomMaterial.LightingModel.clearcoat, and call `params().surface().set_specular()` from its surface shader.

The following Metal code demonstrates using the specular scale and texture values, simulating the behavior of the shaders that render a PhysicallyBasedMaterial:

```
// Retrieve the opacity scale from the CustomMaterial.
float specularScale = params.material_constants().specular_scale();

// Retrieve the entity's texture coordinates.
float2 uv = params.geometry().uv0();

// Entities loaded from a USDZ or .reality file use texture coordinates
// with a flipped y-axis. This compensates for that.
uv.y = 1.0 - uv.y;

// Sample the specular texture.
auto tex = params.textures();
half specular = tex.specular().sample(textureSampler, uv).r;

// Multiply the tint and the sampled value from the texture and assign
// the result.
specular *= specularScale;
params.surface().set_specular(specular);
```

For more information on creating custom materials and writing shader functions, see Modifying RealityKit rendering using custom materials.

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

var ambientOcclusion: CustomMaterial.AmbientOcclusion

The ambient light exposure for a material.

var clearcoat: CustomMaterial.Clearcoat

The transparent highlights that simulate a clear, shiny coating on an entity.

var clearcoatRoughness: CustomMaterial.ClearcoatRoughness

The degree to which an entity’s clear, shiny coating scatters light to create soft highlights.

var clearcoatNormal: CustomMaterial.ClearcoatNormal

Waviness and imperfections for the top clearcoat.

