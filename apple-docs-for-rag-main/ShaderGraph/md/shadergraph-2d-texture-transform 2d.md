

- ShaderGraph
- 2D-Texture
-  Transform 2D 

ShaderGraph Node

# Transform 2D

A node that applies an affine transformation to a 2d input.

## Parameter Types

| Input         | Type     |
|---------------|----------|
| `In`          | Vector2f |
| `Rotation`    | Float    |
| `Scale`       | Vector2f |
| `Translation` | Vector2f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector2f |

## Parameter descriptions

`In`  
The 2D input to be transformed.

`Rotation`  
The degrees of counter-clockwise rotation to apply to the input.

`Scale`  
The scale to apply to the input. This parameter stretches the input by the given magnitude.

`Translation`  
The translation to apply to the input. A translation moves the input in the given directions.

## Discussion

The Transform 2D node takes a 2D vector as an input, applies the given rotation, scale, and translation, and then outputs the transformed vector.

## See Also

### Nodes

Image

A texture referencing a 2D image file.

Tiled Image

Samples data from an image with provisions for offsetting and tiling in UV space.

UV Texture

A MaterialX version of USD UV Texture reader.

