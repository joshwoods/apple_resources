

- RealityKit
- CustomMaterial
-  clearcoatRoughness 

Instance Property

# clearcoatRoughness

The degree to which an entity’s clear, shiny coating scatters light to create soft highlights.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var clearcoatRoughness: CustomMaterial.ClearcoatRoughness { get set }
```

## Discussion

An entity in RealityKit can display a clearcoat, which is a separate layer of transparent specular highlights used to simulate a clear coating, like on a car or the surface of lacquered objects. This property allows you to specify a clearcoat roughness value to indicate how much the clearcoat scatters light that bounces off of it, which softens and disperses the highlights.

You can specify a single value that applies to the entire material, or you can supply a UV-mapped image texture containing different roughness values for different parts of the entity. This value is available in your surface shader. RealityKit won’t render a clearcoat with roughness unless your surface shader calls both `params.surface().set_clearcoat_roughness()` and `params.surface().set_clearcoat()` with a value greater than `0.0`.

The following Swift code demonstrates setting the `clearcoatRoughness` using a single value:

```
material.clearcoatRoughness = .init(floatLiteral: 0.5)
```

This example shows how to set the `clearcoatRoughness` using a UV-mapped image:

```
if let clearcoatRoughnessResource = try?
TextureResource.load(named: "entity_cc_roughness") {
    let ccRoughnessMap = MaterialParameters.Texture(clearcoatRoughnessResource)
    material.clearcoat = .init(texture: ccRoughnessMap)
}
```

With custom materials, RealityKit only renders a clearcoat if lightingModel is CustomMaterial.LightingModel.clearcoat and the material’s surface shader function calls `params.surface().set_clearcoat()`. To specify clearcoatRoughness, your surface shader function needs to also call `params.surface().set_clearcoat_roughness()`.

The following Metal code demonstrates using clearcoat and clearcoatRoughness in a surface shader, replicating the behavior of the PhysicallyBasedMaterial shader:

```
// Retrieve the clearcoat scale and roughness from the CustomMaterial.
float clearcoatScale = params.material_constants().clearcoat_scale();
float clearcoatRoughnessScale = params.material_constants().clearcoat_roughness_scale();

// Retrieve the entity's texture coordinates.
float2 uv = params.geometry().uv0();

// Entities loaded from a USDZ or .reality file use texture coordinates with
// a flipped y-axis. This compensates for that.
uv.y = 1.0 - uv.y;

// Sample a value from the clearcoat and clearcoat roughness textures.
auto tex = params.textures();
half clearcoat = tex.clearcoat().sample(textureSampler, uv).r;
half clearcoatRoughness = tex.clearcoat_roughness().sample(textureSampler, uv).r;

// Multiply the scale and sampled texture value from the clearcoat and
// assign  the result.
clearcoat *= clearcoatScale;
params.surface().set_clearcoat(clearcoat);

// Multiply the scale and sampled texture value from the clearcoat roughness
// and assign the result.
clearcoatRoughness *= clearcoatRoughnessScale;
params.surface().set_clearcoat_roughness(clearcoatRoughness);
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

var ambientOcclusion: CustomMaterial.AmbientOcclusion

The ambient light exposure for a material.

var specular: CustomMaterial.Specular

The bright highlights to apply to the entity.

var clearcoat: CustomMaterial.Clearcoat

The transparent highlights that simulate a clear, shiny coating on an entity.

var clearcoatNormal: CustomMaterial.ClearcoatNormal

Waviness and imperfections for the top clearcoat.

