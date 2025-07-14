

- RealityKit
- CustomMaterial
- CustomMaterial.Clearcoat
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

A clearcoat is a separate layer of transparent specular highlights used to simulate a clear coating, like on a car or the surface of lacquered objects. Use this initializer to create an object to specify the amount of clearcoat for a material using a single value that applies to the entire material.

The clearcoat value is available in the material’s surface shader function, but RealityKit doesn’t render a clearcoat unless the material’s lightingModel is CustomMaterial.LightingModel.clearcoat and its surface shader function calls `params.surface().set_clearcoat()`.

The following Metal code demonstrates how to retrieve the clearcoat scale in a surface shader function and use it to set the final clearcoat value for rendering:

```
    // Retrieve the base color tint from the CustomMaterial.
    float clearcoatScale = params.material_constants().clearcoat_scale();

    // Assign the scale value as the clearcoat value for this pixel.
    params.surface().set_clearcoat(clearcoat);
```

## See Also

### Creating a clearcoat object

init(scale: Float, texture: CustomMaterial.Texture?)

Creates a clearcoat object using a single value or a texture.

init(PhysicallyBasedMaterial.Clearcoat)

Creates a custom clearcoat object from a physically based material’s clearcoat property.

