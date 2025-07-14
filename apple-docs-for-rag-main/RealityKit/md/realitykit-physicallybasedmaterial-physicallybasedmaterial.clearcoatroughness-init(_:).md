

- RealityKit
- PhysicallyBasedMaterial
- PhysicallyBasedMaterial.ClearcoatRoughness
-  init(\_:) 

Initializer

# init(\_:)

Creates a clearcoat roughness object from a custom material’s clearcoat roughness property.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
init(_ value: CustomMaterial.ClearcoatRoughness)
```

## Parameters 

`value`  

The custom material’s clearcoat roughness property.

## Discussion

A clearcoat is a separate layer of transparent specular highlights used to simulate a clear transparent coating, like the paint on a car, or the surface of lacquered objects. When you enable clearcoat rendering for a material, RealityKit renders the clearcoat as a separate layer just above the surface of the entity. You can specify a clearcoat roughness value for the clearcoat to indicate how much the clearcoat scatters light that bounces off of it, which softens and spreads out the highlights.

This initializer creates an object that specifies the clearcoat roughness for a material that uses the clearcoatRoughness property from a CustomMaterial object.

## See Also

### Creating a clearcoat roughness object

init(floatLiteral: Float)

Creates a clearcoat roughness object using a single value.

init(scale: Float, texture: PhysicallyBasedMaterial.Texture?)

Creates a clearcoat roughness object using a single value or a texture.

