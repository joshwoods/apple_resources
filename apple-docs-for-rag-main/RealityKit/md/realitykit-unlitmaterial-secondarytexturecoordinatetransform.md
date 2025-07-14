

- RealityKit
- UnlitMaterial
-  secondaryTextureCoordinateTransform 

Instance Property

# secondaryTextureCoordinateTransform

A two-dimensional transformation to apply to the entity’s secondary texture coordinates.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var secondaryTextureCoordinateTransform: UnlitMaterial.TextureCoordinateTransform { get set }
```

## Discussion

This property transforms the secondary set. To transform the primary UV coordinates in a material, see textureCoordinateTransform.

