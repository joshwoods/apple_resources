

- RealityKit
- PhysicallyBasedMaterial
- PhysicallyBasedMaterial.Specular
-  init(\_:) 

Initializer

# init(\_:)

Creates an object from a custom material’s specular property.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
init(_ value: CustomMaterial.Specular)
```

## Parameters 

`value`  

The custom material’s specular property.

## Discussion

RealityKit automatically draws *specular highlights* for physically based materials using the values of various properties, primarily roughness and metallic. Specular highlights are bright spots of reflected light that appear on shiny objects.

While many real-world objects can be accurately and realistically simulated with just the core PBR properties, you can create additional realistic effects by augmenting the specular highlights.

This initializer creates a PhysicallyBasedMaterial.Specular object from the specular property of a CustomMaterial.

## See Also

### Creating a specular object

init(floatLiteral: Float)

Creates an object from single value.

init(scale: Float, texture: PhysicallyBasedMaterial.Texture?)

Creates an object from a single value or a texture.

