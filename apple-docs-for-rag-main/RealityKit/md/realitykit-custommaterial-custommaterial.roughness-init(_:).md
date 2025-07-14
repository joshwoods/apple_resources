

- RealityKit
- CustomMaterial
- CustomMaterial.Roughness
-  init(\_:) 

Initializer

# init(\_:)

Creates a roughness object from a physically based material’s roughness property.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
init(_ value: PhysicallyBasedMaterial.Roughness)
```

## Parameters 

`value`  

The physically based material’s roughness property.

## Discussion

This initializer creates a roughness object by copying the scale and texture values from an existing PhysicallyBasedMaterial.Roughness object.

With custom materials, the `texture` and `scale` properties of the CustomMaterial.Roughness object are available in your surface shader function, but RealityKit doesn’t automatically use them when rendering your entity. To render an entity with roughness, set lightingModel to CustomMaterial.LightingModel.lit or CustomMaterial.LightingModel.clearcoat, and call `params.surface().set_roughness()` from its surface shader.

To achieve the same roughness behavior as PhysicallyBasedMaterial, the surface shader function multiplies roughness scale by the sampled value from the texture, as the following Metal code demonstrates:

```
    // Retrieve the roughness scale from the CustomMaterial.
    float roughnessScale = params.material_constants().roughness_scale();

    // Retrieve the entity's UV texture coordinates.
    float2 uv = params.geometry().uv0();

    // Models loaded from USDZ or Reality Composer use UVs that are flipped
    // on the y-axis. This compensates for that.
    uv.y = 1.0 - uv.y;

    // Sample the texture based on the resulting UVs.
    auto tex = params.textures();
    half roughness = tex.roughness().sample(textureSampler, uv).r;

    // Multiply the scale and the sampled value from the texture, and assign
    // the result to the shader's base color property.
    roughness *= roughnessScale;

    // Set the roughness value to be used by the custom material shader.
    params.surface().set_roughness(roughness);
```

For more information on creating custom materials and writing shader functions, see Modifying RealityKit rendering using custom materials.

## See Also

### Creating a roughness object

init(floatLiteral: Float)

Creates an object to specify the amount of roughness, using a single value that applies to the entire material.

init(scale: Float, texture: CustomMaterial.Texture?)

Creates a roughness object from a color or texture.

