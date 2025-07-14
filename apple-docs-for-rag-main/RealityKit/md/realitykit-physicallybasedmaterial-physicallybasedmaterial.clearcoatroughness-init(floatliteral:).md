

- RealityKit
- PhysicallyBasedMaterial
- PhysicallyBasedMaterial.ClearcoatRoughness
-  init(floatLiteral:) 

Initializer

# init(floatLiteral:)

Creates a clearcoat roughness object using a single value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
init(floatLiteral value: Float)
```

## Parameters 

`value`  

The clearcoat roughness value to use for the entire material.

## Discussion

A clearcoat is a separate layer of transparent specular highlights used to simulate a clear transparent coating, like the paint on a car, or the surface of lacquered objects. When you enable clearcoat rendering for a material, RealityKit renders the clearcoat as a separate layer just above the surface of the entity. You can specify a clearcoat roughness value for the clearcoat to indicate how much the clearcoat scatters light that bounces off of it, which softens and spreads out the highlights.

This initializer creates an object that specifies the clearcoat roughness for a material using a single value for the entire material.

## See Also

### Creating a clearcoat roughness object

init(scale: Float, texture: PhysicallyBasedMaterial.Texture?)

Creates a clearcoat roughness object using a single value or a texture.

init(CustomMaterial.ClearcoatRoughness)

Creates a clearcoat roughness object from a custom material’s clearcoat roughness property.

