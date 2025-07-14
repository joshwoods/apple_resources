

- RealityKit
- PhysicallyBasedMaterial
- PhysicallyBasedMaterial.Clearcoat
-  init(floatLiteral:) 

Initializer

# init(floatLiteral:)

Creates a clearcoat object using a single value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
init(floatLiteral value: Float)
```

## Parameters 

`value`  

The clearcoat value to use for the entity.

## Discussion

A clearcoat is a separate layer of transparent specular highlights used to simulate a clear transparent coating, like the paint on a car, or the surface of lacquered objects. Use this initializer to create an object to specify the amount of clearcoat for a material using a single value that applies to the entire material.

## See Also

### Creating a clearcoat object

init(scale: Float, texture: PhysicallyBasedMaterial.Texture?)

Creates a clearcoat object using a single value or a texture.

init(CustomMaterial.Clearcoat)

Creates a clearcoat object from a custom material’s clearcoat property.

