

- RealityKit
- CustomMaterial
-  baseColor 

Instance Property

# baseColor

The color of an entity unmodified by lighting.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var baseColor: CustomMaterial.BaseColor { get set }
```

## Discussion

In physically based rendering, the base color of an entity is its color before RealityKit applies any lighting calculations or other rendering calculations to it. With custom materials, the base color `texture` and `tint` are available as inputs in your surface shader. With custom materials, RealityKit doesn’t automatically use the values set on the baseColor property. The material’s surface shader is responsible for calculating or setting the actual base color value for rendering by calling `params.surface().set_base_color()`.

The following code shows how to create a base color from a tint color and a texture, and then assign it to a custom material:

```
// Load entity_basecolor.jpg from the app's bundle.
if let baseResource = try? TextureResource.load(named: "entity_basecolor") {
    let baseColor = CustomMaterial.Texture(baseResource)
    customMaterial.baseColor = CustomMaterial.BaseColor(tint: .blue,
                                                        texture:baseColor)
}
```

In your surface shader, you can access the `tint` of the material’s base color property by calling `params.material_constants().base_color_tint()`. You can access the texture by calling `params.textures().base_color()`.

The following surface shader function takes the tint and texture values from the baseColor property, multiplies them together, and sets the resulting value as the base color for rendering, which emulates the behavior of PhysicallyBasedMaterial:

```
#include 
#include 
using namespace metal;

// Use samplers to retrieve a color value from a texture based on // UV
coordinates. Samplers can be reused with different textures. //
RealityKit reserves eight samplers for itself, so surface shaders should
// never define more than eight samplers. constexpr sampler
textureSampler(address::clamp_to_edge, filter::bicubic);

[[visible]] void mySurfaceShader(realitykit::surface_parameters params)
{
    // Retrieve the base color tint from the CustomMaterial.
    half3 baseColorTint = (half3)params.material_constants().base_color_tint();

    // Sample a value from the CustomMaterial's base color texture
    // using the entity's UV coordinates.
    auto uv = params.geometry().uv0();
    auto tex = params.textures();
    half3 color = (half3)tex.base_color().sample(textureSampler, uv).rgb;

    // Multiply the tint and color sampled from the base color texture and
    // assign the result to the shader's base color property.
    color *= baseColorTint;
    params.surface().set_base_color(color);
}
```

For more information on creating custom materials and writing shader functions, see Modifying RealityKit rendering using custom materials.

## See Also

### Setting the core properties

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

var specular: CustomMaterial.Specular

The bright highlights to apply to the entity.

var clearcoat: CustomMaterial.Clearcoat

The transparent highlights that simulate a clear, shiny coating on an entity.

var clearcoatRoughness: CustomMaterial.ClearcoatRoughness

The degree to which an entity’s clear, shiny coating scatters light to create soft highlights.

var clearcoatNormal: CustomMaterial.ClearcoatNormal

Waviness and imperfections for the top clearcoat.

