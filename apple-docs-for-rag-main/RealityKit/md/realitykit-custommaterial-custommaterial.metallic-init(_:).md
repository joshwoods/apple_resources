

- RealityKit
- CustomMaterial
- CustomMaterial.Metallic
-  init(\_:) 

Initializer

# init(\_:)

Creates a metallic object from a physically based material’s metallic property.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
init(_ value: PhysicallyBasedMaterial.Metallic)
```

## Parameters 

`value`  

The physically based material’s metallic property.

## Discussion

This initializer creates a new object by copying the values from an existing PhysicallyBasedMaterial.Metallic object.

To render an entity with reflectiveness, set lightingModel to CustomMaterial.LightingModel.lit or CustomMaterial.LightingModel.clearcoat, and call `params.surface().set_metallic()` from its surface shader function.

To achieve the same metallic behavior as PhysicallyBasedMaterial, the surface shader function multiplies metallic scale by the sampled value from the texture, as the following Metal code demonstrates:

```
    // Retrieve the metallic scale from the CustomMaterial.
    float metallicScale = params.material_constants().metallic_scale();

    // Retrieve the entity's UV texture coordinates.
    float2 uv = params.geometry().uv0();

    // Models loaded from USDZ or Reality Composer use UVs that are flipped
    // on the y-axis. This compensates for that.
    uv.y = 1.0 - uv.y;

    // Sample the texture based on the resulting UVs.
    auto tex = params.textures();
    half metallic = tex.metallic().sample(textureSampler, uv).r;

    // Multiply the scale and the sampled value from the texture,
    // and assign the result to the shader's metallic property.
    metallic *= metallicScale;
    params.surface().set_metallic(metallic);
```

For more information on creating custom materials and writing shader functions, see Modifying RealityKit rendering using custom materials.

## See Also

### Creating a metallic object

init(floatLiteral: Float)

Creates an object from a single value.

init(scale: Float, texture: CustomMaterial.Texture?)

Creates an object from a color or texture.

