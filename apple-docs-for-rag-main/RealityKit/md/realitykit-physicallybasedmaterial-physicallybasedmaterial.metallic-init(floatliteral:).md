

- RealityKit
- PhysicallyBasedMaterial
- PhysicallyBasedMaterial.Metallic
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

The reflectiveness value for the material.

## Discussion

In PBR rendering, the `metallic` property represents the reflectiveness of an entity. This initializer creates a new object from a single value to describe the reflectiveness of the entire material. A value of 0.0 creates a *dielectric* (or non-reflective) material. Values greater than 0.0 result in an increasingly *metallic* (or reflective) materials.

## See Also

### Creating a metallic object

init(scale: Float, texture: PhysicallyBasedMaterial.Texture?)

Creates an object from a color or texture.

init(CustomMaterial.Metallic)

Creates a metallic object from a custom material’s metallic property.

