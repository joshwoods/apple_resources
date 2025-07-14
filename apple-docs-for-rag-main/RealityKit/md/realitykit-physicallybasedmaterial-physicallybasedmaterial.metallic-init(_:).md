

- RealityKit
- PhysicallyBasedMaterial
- PhysicallyBasedMaterial.Metallic
-  init(\_:) 

Initializer

# init(\_:)

Creates a metallic object from a custom material’s metallic property.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
init(_ value: CustomMaterial.Metallic)
```

## Parameters 

`value`  

The custom material’s metallic property.

## Discussion

In PBR rendering, the `metallic` property represents the reflectiveness of an entity. This initializer creates a new object from the metallic property of a CustomMaterial.

## See Also

### Creating a metallic object

init(floatLiteral: Float)

Creates an object from single value.

init(scale: Float, texture: PhysicallyBasedMaterial.Texture?)

Creates an object from a color or texture.

