

- RealityKit
- CustomMaterial
- CustomMaterial.ClearcoatRoughness
-  init(\_:) 

Initializer

# init(\_:)

Creates a custom clearcoat object from a physically based material’s clearcoat property.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
init(_ value: PhysicallyBasedMaterial.ClearcoatRoughness)
```

## Parameters 

`value`  

The clearcoatRoughness property from a PhysicallyBasedMaterial.

## Discussion

This initializer creates a new object by copying the scale and texture values from an existing PhysicallyBasedMaterial.ClearcoatRoughness object.

A clearcoat is a separate layer of transparent specular highlights used to simulate a clear coating, like on a car or the surface of lacquered objects. Use this initializer to create an object to specify the amount of clearcoat for a material using a single value for the entire material, a UV-mapped image to specify different values for different parts of the entity, or both.

The values from this property are available in the custom material’s surface shader function regardless of the value of lightingModel , but clearcoat isn’t drawn unless the custom material’s lightingModel is CustomMaterial.LightingModel.clearcoat and the surface shader calls `params.surface().set_clearcoat()`.

The following Metal code demonstrates how to retrieve `scale` and `texture` in a surface shader, and use them to specify the clearcoat and clearcoat roughness values:

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
    half clearcoatRoughess = tex.clearcoat_roughness().sample(textureSampler, uv).r;

    // Multiply the scale and sampled texture value from the clearcoat,
    // and assign the result.
    clearcoat *= clearcoatScale;
    params.surface().set_clearcoat(clearcoat);

    // Multiply the scale and sampled texture value from the clearcoat roughness,
    // and assign the result.
    clearcoatRoughess *= clearcoatRoughnessScale;
    params.surface().set_clearcoat_roughness(clearcoatRoughess);
```

## See Also

### Creating a clearcoat roughness object

init(floatLiteral: Float)

Creates a clearcoat object using a single value.

init(scale: Float, texture: CustomMaterial.Texture?)

Creates a clearcoat object using a single value or a texture.

