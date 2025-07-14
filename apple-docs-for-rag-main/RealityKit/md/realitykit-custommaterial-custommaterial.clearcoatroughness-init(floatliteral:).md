

- RealityKit
- CustomMaterial
- CustomMaterial.ClearcoatRoughness
-  init(floatLiteral:) 

Initializer

# init(floatLiteral:)

Creates a clearcoat object using a single value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
init(floatLiteral value: Float)
```

## Parameters 

`value`  

The clearcoat value to use for the entity.

## Discussion

A clearcoat is a separate layer of transparent specular highlights used to simulate a clear coating, like on a car or the surface of lacquered objects. Use this initializer to create an object to specify the amount of clearcoat for a material using a single value for the entire material, a UV-mapped image to specify different values for different parts of the entity, or both.

The values from this property are available in the custom material’s surface shader function regardless of the value of lightingModel , but clearcoat isn’t drawn unless the custom material’s lightingModel is CustomMaterial.LightingModel.clearcoat and the surface shader calls `params.surface().set_clearcoat()`.

The following Metal code demonstrates how to retrieve the scale and texture values from this property and use them to enable clearcoat rendering.

```
    // Retrieve the clearcoat scale and roughness from the CustomMaterial.
    float clearcoatScale = params.material_constants().clearcoat_scale();
    float clearcoatRoughnessScale = params.material_constants().clearcoat_roughness_scale();

    // Assign the clearcoat scale to enable clearcoat rendering (if
    // lightingModel is .clearcoat).
    params.surface().set_clearcoat(clearcoatScale);

    // Assign the clearcoat roughness from the scale property set
    //  on the custom material.
    params.surface().set_clearcoat_roughness(clearcoatRoughnessScale);
```

## See Also

### Creating a clearcoat roughness object

init(scale: Float, texture: CustomMaterial.Texture?)

Creates a clearcoat object using a single value or a texture.

init(PhysicallyBasedMaterial.ClearcoatRoughness)

Creates a custom clearcoat object from a physically based material’s clearcoat property.

