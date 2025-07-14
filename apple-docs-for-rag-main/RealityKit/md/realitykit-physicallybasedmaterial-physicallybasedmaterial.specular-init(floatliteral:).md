

- RealityKit
- PhysicallyBasedMaterial
- PhysicallyBasedMaterial.Specular
-  init(floatLiteral:) 

Initializer

# init(floatLiteral:)

Creates an object from single value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
init(floatLiteral value: Float)
```

## Parameters 

`value`  

A value from 0.0 to 1.0 to use as the specular value for the material.

## Discussion

RealityKit automatically draws *specular highlights* for physically based materials using the values of various properties, primarily roughness and metallic. Specular highlights are bright spots of reflected light that appear on shiny objects.

While many real-world objects can be accurately and realistically simulated with just the core PBR properties, you can create additional realistic effects by augmenting the specular highlights.

This initializer creates a PhysicallyBasedMaterial.Specular object from a single value that applies to the entire material.

## See Also

### Creating a specular object

init(scale: Float, texture: PhysicallyBasedMaterial.Texture?)

Creates an object from a single value or a texture.

init(CustomMaterial.Specular)

Creates an object from a custom material’s specular property.

