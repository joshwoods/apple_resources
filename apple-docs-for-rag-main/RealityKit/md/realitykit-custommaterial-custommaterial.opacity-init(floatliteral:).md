

- RealityKit
- CustomMaterial
- CustomMaterial.Opacity
-  init(floatLiteral:) 

Initializer

# init(floatLiteral:)

Creates an opacity object from a single value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
init(floatLiteral value: Float)
```

## Parameters 

`value`  

The opacity value.

## Discussion

This initializer creates an object that defines the opacity of an entity using a single value for the entire entity. This value is available to the material’s surface shader function, but RealityKit draws the entity fully opaque unless the surface shader function calls `params.surface().set_opacity()`.

The following Metal code demonstrates how to set the entity’s opacity in the material’s surface shader function based on `value:`

```
    // Retrieve the opacity scale from the CustomMaterial.
    float opacityScale = params.material_constants().opacity_scale();

    // Use the opacity scale to set the current pixel's opacity.
    params.surface().set_opacity(opacityScale);
```

## See Also

### Creating an opacity object

init(scale: Float, texture: CustomMaterial.Texture?)

Creates an object that defines the opacity of an entity using a single value, a UV-mapped image texture, or both.

init(PhysicallyBasedMaterial.Opacity)

Creates an object from the opacity property of an existing physically based material.

