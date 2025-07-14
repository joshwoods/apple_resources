

- RealityKit
- CustomMaterial
-  clearcoat 

Instance Property

# clearcoat

The transparent highlights that simulate a clear, shiny coating on an entity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var clearcoat: CustomMaterial.Clearcoat { get set }
```

## Discussion

An entity in RealityKit can display a clearcoat, which is a separate layer of transparent specular highlights used to simulate a clear coating, like on a car or the surface of lacquered objects.

This property allows you to specify clearcoat using a single `Float` that applies to the entire material, or a UV-mapped grayscale image to provide different values for different parts of an entity.

The following example specifies `clearcoat` using a single value:

```
material.clearcoat = .init(floatLiteral: 0.8)
```

This example shows how to specify `clearcoat` using a UV-mapped image texture:

```
if let clearcoatResource = try? TextureResource.load(named:
"entity_clearcoat") {
    let clearcoatMap = MaterialParameters.Texture(clearcoatResource)
    material.clearcoat = .init(texture: clearcoatMap)
}
```

With custom materials, RealityKit doesn’t automatically use the values you set for this property to render your entity. The values from this property are available to the custom material’s surface shader, but it doesn’t render a clearcoat unless the custom material’s lightingModel is CustomMaterial.LightingModel.clearcoat and the surface shader calls `params.surface().set_clearcoat()`.

The following Metal code demonstrates how to retrieve the scale and texture from this property, and use them to enable clearcoat rendering.

```
// Retrieve the clearcoat scale from the CustomMaterial.
float clearcoatScale = params.material_constants().clearcoat_scale();

// Retrieve the entity's texture coordinates.
float2 uv = params.geometry().uv0();

// Models loaded from USDZ or .reality files use texture coordinates with a
// flipped y-axis. This compensates for that.
uv.y = 1.0 - uv.y;

// Sample the clearcoat texture using the texture coordinates.
auto tex = params.textures();
half clearcoat = tex.clearcoat().sample(textureSampler, uv).r;

// Multiply the scale and sampled value from the texture, and assign
// the result.
clearcoat *= clearcoatScale;
params.surface().set_clearcoat(clearcoat);
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

var clearcoatRoughness: CustomMaterial.ClearcoatRoughness

The degree to which an entity’s clear, shiny coating scatters light to create soft highlights.

var clearcoatNormal: CustomMaterial.ClearcoatNormal

Waviness and imperfections for the top clearcoat.

