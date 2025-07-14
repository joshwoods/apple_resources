

- RealityKit
- CustomMaterial
- CustomMaterial.Metallic
-  init(floatLiteral:) 

Initializer

# init(floatLiteral:)

Creates an object from a single value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
init(floatLiteral value: Float)
```

## Parameters 

`value`  

The reflectiveness value for the material.

## Discussion

In physically based rendering, the `metallic` property represents the reflectiveness of an entity. This initializer creates a new object that passes a single metallic value to your custom shader functions but doesn’t pass a texture.

The following Swift code shows how to specify reflectiveness using a single value for the entire entity:

```
material.roughness = PhysicallyBasedMaterial.Roughness(floatLiteral: 0.0)
```

To render an entity with reflectiveness, set lightingModel to CustomMaterial.LightingModel.lit or CustomMaterial.LightingModel.clearcoat, and call `params.surface().set_metallic()` from its surface shader.

The following Metal code shows how to retrieve the value set in this initializer in your surface shader and use it:

```
    // Retrieve the metallic scale from the CustomMaterial.
    float metallic = params.material_constants().metallic_scale();

    // Set the roughness value using the metallic scale value.
    params.surface().set_metallic(metallic);
```

For more information on creating custom materials and writing shader functions, see Modifying RealityKit rendering using custom materials.

## See Also

### Creating a metallic object

init(scale: Float, texture: CustomMaterial.Texture?)

Creates an object from a color or texture.

init(PhysicallyBasedMaterial.Metallic)

Creates a metallic object from a physically based material’s metallic property.

