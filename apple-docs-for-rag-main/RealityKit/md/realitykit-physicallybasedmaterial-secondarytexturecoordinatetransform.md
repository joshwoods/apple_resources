

- RealityKit
- PhysicallyBasedMaterial
-  secondaryTextureCoordinateTransform 

Instance Property

# secondaryTextureCoordinateTransform

A two-dimensional transformation to apply to the entity’s secondary texture coordinates.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var secondaryTextureCoordinateTransform: PhysicallyBasedMaterial.TextureCoordinateTransform { get set }
```

## Discussion

An entity’s UV texture coordinates define how RealityKit maps image textures onto an entity. This property allows you to transform the secondary texture coordinates to change the way this material maps textures onto an entity. If an entity has multiple materials assigned to it, the transformation doesn’t affect how the other materials map their textures.

You might, for example, change the scale of the UV coordinates to apply a tiled, repeating pattern to the surface of your entity, or continuously rotate or translate the texture coordinates to animate materials to create special effects, such as fire or flowing liquids.

The following example demonstrates how to set a material’s UV transformation:

```
let rotationRadians = Float(45.0) * .pi / 180 // 45 degrees converted to radians.
secondaryTextureCoordinateTransform =.init(offset: SIMD2(x:0.5, y: 0.5),
                                            scale: SIMD2(x:0.5, y: 0.5),
                                            rotation: rotationRadians)
```

Some entities imported from USDZ files have more than one set of UV coordinates. This property transforms the secondary set. To transform the primary UV coordinates in a material, see textureCoordinateTransform.

## See Also

### Modifying texture coordinates

var textureCoordinateTransform: PhysicallyBasedMaterial.TextureCoordinateTransform

A two-dimensional transformation to apply to the entity’s primary texture coordinates.

