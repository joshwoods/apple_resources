

- RealityKit
- CustomMaterial
- CustomMaterial.Specular
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

A value from `0.0` to `1.0` to use as the specular value for the material.

## Discussion

RealityKit automatically draws *specular highlights* for physically based materials using the values of various properties, primarily roughness and metallic. Specular highlights are bright spots of reflected light that appear on shiny objects.

While many real-world objects can be accurately and realistically simulated with just the core physically based rendering (PBR) properties, you can create additional realistic effects by augmenting the specular highlights.

This initializer creates a PhysicallyBasedMaterial.Specular object from a single value that applies to the entire material. The specular scale value is available to the material’s surface shader, but RealityKit doesn’t create additional specular highlights unless the surface shader function calls `params.surface().set_specular()`.

The following Metal code demonstrates using the specular `scale` value in a surface shader function:

```
    // Retrieve the opacity scale from the CustomMaterial and assign it.
    float specularScale = params.material_constants().specular_scale();
    params.surface().set_specular(specular);
```

## See Also

### Creating a specular object

init(scale: Float, texture: CustomMaterial.Texture?)

Creates an object from a single value, a UV-mapped texture, or both.

init(PhysicallyBasedMaterial.Specular)

Creates an object from a physically based material’s specular property.

