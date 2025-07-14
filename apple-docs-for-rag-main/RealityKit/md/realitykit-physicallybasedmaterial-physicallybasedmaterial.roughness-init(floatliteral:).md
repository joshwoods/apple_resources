

- RealityKit
- PhysicallyBasedMaterial
- PhysicallyBasedMaterial.Roughness
-  init(floatLiteral:) 

Initializer

# init(floatLiteral:)

Creates an object from a single value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
init(floatLiteral value: Float)
```

## Parameters 

`value`  

The roughness value.

## Discussion

The `roughness` property represents how much the surface of the entity scatters light it reflects. A material with a high roughness has a matte appearance, while one with a low roughness has a shiny appearance.

Use this initializer to create an object to specify the amount of roughness using a single value that applies to the entire material.

## See Also

### Creating a roughness object

init(scale: Float, texture: PhysicallyBasedMaterial.Texture?)

Creates a roughness object from a color or texture.

init(CustomMaterial.Roughness)

Creates a roughness object from a custom material’s roughness property.

