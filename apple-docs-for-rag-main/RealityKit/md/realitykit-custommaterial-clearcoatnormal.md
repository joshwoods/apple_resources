

- RealityKit
- CustomMaterial
-  clearcoatNormal 

Instance Property

# clearcoatNormal

Waviness and imperfections for the top clearcoat.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
var clearcoatNormal: CustomMaterial.ClearcoatNormal { get set }
```

## Discussion

An entity in RealityKit can display a clearcoat, which is a separate layer of transparent specular highlights used to simulate a clear coating, like on a car or the surface of lacquered objects. This property allows you to specify a clearcoat normal and add waviness and imperfections to the top clearcoat.

This example shows how to set the `clearcoatNormal` using a UV-mapped image:

```
if let clearcoatNormalTextureResource = try?
TextureResource.load(named: "entity_cc_normalMap") {
    let ccNormalMap = CustomMaterial.Texture(clearcoatNormalTextureResource)
    material.clearcoatNormal = .init(texture: ccNormalMap)
}
```

With custom materials, RealityKit only renders a clearcoat if lightingModel is CustomMaterial.LightingModel.clearcoat and the material’s surface shader function calls `params.surface().set_clearcoat()`. To specify clearcoatNormal, your surface shader function also needs to call `params.surface().set_clearcoat_normal()`.

The following Metal code demonstrates using clearcoat and clearcoatNormal in a surface shader, replicating the behavior of the PhysicallyBasedMaterial shader:

```
// Retrieve the entity's texture coordinates.
float2 uv = params.geometry().uv0();

// Entities loaded from a USDZ or .reality file use texture coordinates with
// a flipped y-axis. This compensates for that.
uv.y = 1.0 - uv.y;

// Sample a value from the clearcoat normal texture.
auto tex = params.textures();
half3 clearcoatNormal = realitykit::unpack_normal(tex.clearcoat_normal().sample(textureSampler, uv).rgb);

// assign the result.
params.surface().set_clearcoat_normal(clearcoatNormal);
params.surface().set_clearcoat(1.0);
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

var clearcoatRoughness: CustomMaterial.ClearcoatRoughness

The degree to which an entity’s clear, shiny coating scatters light to create soft highlights.

