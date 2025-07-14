

- RealityKit
- CustomMaterial
- CustomMaterial.Roughness
-  init(floatLiteral:) 

Initializer

# init(floatLiteral:)

Creates an object to specify the amount of roughness, using a single value that applies to the entire material.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
init(floatLiteral value: Float)
```

## Parameters 

`value`  

The roughness value.

## Discussion

The `roughness` property represents how much the surface of the entity scatters light that it reflects. A material with a high roughness has a matte appearance, and one with a low roughness has a shiny appearance.

The following Swift code shows how to specify roughness using a single value for the entire entity:

```
material.roughness = PhysicallyBasedMaterial.Roughness(floatLiteral: 0.0)
```

With custom materials, the roughness value is available in your surface shader; however, RealityKit doesn’t use it automatically to render the entity. To render an entity with roughness, the material’s lightingModel needs to be CustomMaterial.LightingModel.lit or CustomMaterial.LightingModel.clearcoat, and call `params.surface().set_roughness()` from its surface shader function.

The following Metal code shows how to retrieve the roughness value set using this initializer in your surface shader:

```
    // Retrieve the roughness scale from the CustomMaterial.
    float roughnessScale = params.material_constants().roughness_scale();

    // Set the roughness value using the roughness scale.
    params.surface().set_roughness(roughnessScale);
```

For more information on creating custom materials and writing shader functions, see Modifying RealityKit rendering using custom materials.

## See Also

### Creating a roughness object

init(scale: Float, texture: CustomMaterial.Texture?)

Creates a roughness object from a color or texture.

init(PhysicallyBasedMaterial.Roughness)

Creates a roughness object from a physically based material’s roughness property.

