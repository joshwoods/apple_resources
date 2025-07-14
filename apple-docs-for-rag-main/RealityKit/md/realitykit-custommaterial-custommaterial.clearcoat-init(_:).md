

- RealityKit
- CustomMaterial
- CustomMaterial.Clearcoat
-  init(\_:) 

Initializer

# init(\_:)

Creates a custom clearcoat object from a physically based material’s clearcoat property.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
init(_ value: PhysicallyBasedMaterial.Clearcoat)
```

## Parameters 

`value`  

The clearcoat property from a PhysicallyBasedMaterial.

## Discussion

This initializer creates an object by copying the scale and texture values from the clearcoat property of a PhysicallyBasedMaterial.

A clearcoat is a separate layer of transparent specular highlights used to simulate a clear coating, like on a car or the surface of lacquered objects. Use this initializer to create an object to specify the amount of clearcoat for a material using a single value for the entire material, a UV-mapped image to specify different values for different parts of the entity, or both.

The copied values for scale and texture are available in the material’s surface shader function, regardless of the material’s lighting model; however RealityKit only renders a clearcoat when lightingModel is CustomMaterial.LightingModel.clearcoat and the material’s surface shader function calls `params.surface().set_clearcoat()`.

The following Metal code demonstrates how to retrieve the clearcoat `scale` and `texture` values in a surface shader, and use them to calculate the final clearcoat value for rendering:

```
    // Retrieve the base color tint from the CustomMaterial.
    float clearcoatScale = params.material_constants().clearcoat_scale();

    // Retrieve the entity's primary texture coordinates.
    float2 uv = params.geometry().uv0();

    // Models loaded from a USDZ of .reality file use texture coordinates
    // with a flipped y-axis. This compensates for that.
    uv.y = 1.0 - uv.y;

    // Sample the clearcoat texture to get the value UV-mapped to this pixel.
    auto tex = params.textures();
    half clearcoat = tex.clearcoat().sample(textureSampler, uv).r;

    // Multiply the tint and the sampled value from the texture, and assign it
    // to the shader's base color property.
    clearcoat *= clearcoatScale;
    params.surface().set_clearcoat(clearcoat);
```

## See Also

### Creating a clearcoat object

init(floatLiteral: Float)

Creates a clearcoat object using a single value.

init(scale: Float, texture: CustomMaterial.Texture?)

Creates a clearcoat object using a single value or a texture.

