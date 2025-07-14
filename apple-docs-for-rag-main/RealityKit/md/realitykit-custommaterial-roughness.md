

- RealityKit
- CustomMaterial
-  roughness 

Instance Property

# roughness

The amount the surface of the 3D object scatters reflected light.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var roughness: CustomMaterial.Roughness { get set }
```

## Discussion

In physically based rendering, the `roughness` property represents how much the surface of an entity scatters the light that it reflects. A material with a high roughness has a matte appearance, whereas one with a low roughness has a shiny appearance. With custom materials, RealityKit doesn’t automatically use the values set on this property. To render a custom material using roughness, set lightingModel to CustomMaterial.LightingModel.lit or CustomMaterial.LightingModel.clearcoat, and specify a roughness value by calling `params.surface().set_roughness()` from the surface shader.

With custom materials, the `texture` and `scale` values from the roughness property are available in your surface shader function, but RealityKit doesn’t automatically use them to render your entity. Your surface shader is responsible for calculating or setting the actual roughness value for rendering.

The following example shows how to use an image and a scale value to specify roughness:

```
if let roughnessResource = try? TextureResource.load(named: "entity_roughness") {
    let roughness = MaterialParameters.Texture(roughnessResource)
    material.roughness = PhysicallyBasedMaterial.Roughness(tint: .green, texture:roughness)
}
```

The following surface shader takes the scale and texture from the roughness property, multiplies them together, and sets the resulting value as the roughness for rendering, which emulates the behavior of PhysicallyBasedMaterial:

```
#include 
#include 
using namespace metal;

// Samplers are used to retrieve a color value from a texture based on
// the entity's UV coordinates. Samplers can be reused with different textures.
// Surface shader functions should define no more than eight samplers.
constexpr sampler textureSampler(address::clamp_to_edge, filter::bicubic);

[[visible]] void mySurfaceShader(realitykit::surface_parameters params)
{
    // Retrieve the roughness scale from the CustomMaterial.
    float roughnessScale = params.material_constants().roughness_scale();

    // Retrieve the sampled value from the CustomMaterial's base color texture.
    auto uv = getFlippedUVs(params);
    auto tex = params.textures();
    half roughness = tex.roughness().sample(textureSampler, uv).r;

    // Multiply the tint and the sampled value from the texture, and assign it
    // to the shader's base color property.
    roughness *= roughnessScale;

    // Set the roughness value to be used by the custom material shader.
    params.surface().set_roughness(roughness);
}
```

For more information on creating custom materials and writing shader functions, see Modifying RealityKit rendering using custom materials.

## See Also

### Setting the core properties

var baseColor: CustomMaterial.BaseColor

The color of an entity unmodified by lighting.

var metallic: CustomMaterial.Metallic

The reflectiveness of an entity.

var normal: CustomMaterial.Normal

A texture map that stores fine surface details for the entity.

var emissiveColor: CustomMaterial.EmissiveColor

The color of light this material emits.

var ambientOcclusion: CustomMaterial.AmbientOcclusion

The ambient light exposure for a material.

var specular: CustomMaterial.Specular

The bright highlights to apply to the entity.

var clearcoat: CustomMaterial.Clearcoat

The transparent highlights that simulate a clear, shiny coating on an entity.

var clearcoatRoughness: CustomMaterial.ClearcoatRoughness

The degree to which an entity’s clear, shiny coating scatters light to create soft highlights.

var clearcoatNormal: CustomMaterial.ClearcoatNormal

Waviness and imperfections for the top clearcoat.

