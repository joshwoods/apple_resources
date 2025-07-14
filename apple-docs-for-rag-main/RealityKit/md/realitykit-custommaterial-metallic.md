

- RealityKit
- CustomMaterial
-  metallic 

Instance Property

# metallic

The reflectiveness of an entity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var metallic: CustomMaterial.Metallic { get set }
```

## Discussion

In physically based rendering, the `metallic` property represents the reflectiveness of an entity. Use this property to specify whether the entity displays metallic qualities and reflects the surrounding environment, or displays dielectric qualities and doesn’t reflect the environment. With custom materials, RealityKit doesn’t automatically use the values set on this property. To render a custom material using the metallic property, set lightingModel to CustomMaterial.LightingModel.lit or CustomMaterial.LightingModel.clearcoat and call `params.surface().set_roughness()` from its surface shader.

The following Swift code shows how to use an image and a scale to specify roughness:

```
if let metallicResource = try? TextureResource.load(named:"entity_metallic") {
    let metallic = MaterialParameters.Texture(metallicResource)
    material.metallic = PhysicallyBasedMaterial.Metallic(scale: 1.0, texture:metallic)
}
```

The following surface shader takes the scale and texture values from the metallic property, multiplies them together, and uses the result to specify the metallic value for rendering, which emulates the behavior of PhysicallyBasedMaterial.

```
#include 
#include 
using namespace metal;

// Use samplers to retrieve a color value from a texture based on // the
entity's UV coordinates. Samplers can be reused with different textures.
// Surface shader functions should define no more than eight samplers.
constexpr sampler textureSampler(address::clamp_to_edge,
filter::bicubic);

[[visible]] void mySurfaceShader(realitykit::surface_parameters params)
{
    // Retrieve the metallic scale from the CustomMaterial.
    float metallicScale = params.material_constants().metallic_scale();

    // Retrieve the entity's texture coordinates.
    float2 uv = params.geometry().uv0();

    // Entities loaded from USDZ or .reality files have texture coordinates
    // with a flipped y-axis. This adjusts for that.
    uv.y = 1.0 - uv.y;

    // Sample the metallic texture based on the UV coordinates.
    auto tex = params.textures();
    half metallic = tex.metallic().sample(textureSampler, uv).r;

    // Multiply the tint and the sampled value from the texture,
    // and assign the result to the shader's metallic property.
    metallic *= metallicScale;
    params.surface().set_metallic(metallic);
}
```

For more information on creating custom materials and writing shader functions, see Modifying RealityKit rendering using custom materials.

## See Also

### Setting the core properties

var baseColor: CustomMaterial.BaseColor

The color of an entity unmodified by lighting.

var roughness: CustomMaterial.Roughness

The amount the surface of the 3D object scatters reflected light.

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

