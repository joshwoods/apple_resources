

- ShaderGraph
- 2D-Texture
-  Tiled Image 

ShaderGraph Node

# Tiled Image

Samples data from an image with provisions for offsetting and tiling in UV space.

## Parameter Types

- Tiled Image (float)
- Tiled Image (vector4f)
- Tiled Image (color4f)
- Tiled Image (half)
- Tiled Image (vector2f)
- Tiled Image (color3f)
- Tiled Image (vector3f)

| Input                   | Type      |
|-------------------------|-----------|
| `File`                  | AssetPath |
| `Default`               | Float     |
| `Texture Coordinates`   | Vector2f  |
| `UV Tiling`             | Vector2f  |
| `UV Offset`             | Vector2f  |
| `Real World Image Size` | Vector2f  |
| `Real World Tile Size`  | Vector2f  |
| `Filter Type`           | String    |

| Output | Type  |
|--------|-------|
| `Out`  | Float |

| Input                   | Type      |
|-------------------------|-----------|
| `File`                  | AssetPath |
| `Default`               | Vector4f  |
| `Texture Coordinates`   | Vector2f  |
| `UV Tiling`             | Vector2f  |
| `UV Offset`             | Vector2f  |
| `Real World Image Size` | Vector2f  |
| `Real World Tile Size`  | Vector2f  |
| `Filter Type`           | String    |

| Output | Type     |
|--------|----------|
| `Out`  | Vector4f |

| Input                   | Type      |
|-------------------------|-----------|
| `File`                  | AssetPath |
| `Default`               | Color4    |
| `Texture Coordinates`   | Vector2f  |
| `UV Tiling`             | Vector2f  |
| `UV Offset`             | Vector2f  |
| `Real World Image Size` | Vector2f  |
| `Real World Tile Size`  | Vector2f  |
| `Filter Type`           | String    |

| Output | Type   |
|--------|--------|
| `Out`  | Color4 |

| Input                   | Type      |
|-------------------------|-----------|
| `File`                  | AssetPath |
| `Default`               | Half      |
| `Texture Coordinates`   | Vector2f  |
| `UV Tiling`             | Vector2f  |
| `UV Offset`             | Vector2f  |
| `Real World Image Size` | Vector2f  |
| `Real World Tile Size`  | Vector2f  |
| `Filter Type`           | String    |

| Output | Type |
|--------|------|
| `Out`  | Half |

| Input                   | Type      |
|-------------------------|-----------|
| `File`                  | AssetPath |
| `Default`               | Vector2f  |
| `Texture Coordinates`   | Vector2f  |
| `UV Tiling`             | Vector2f  |
| `UV Offset`             | Vector2f  |
| `Real World Image Size` | Vector2f  |
| `Real World Tile Size`  | Vector2f  |
| `Filter Type`           | String    |

| Output | Type     |
|--------|----------|
| `Out`  | Vector2f |

| Input                   | Type      |
|-------------------------|-----------|
| `File`                  | AssetPath |
| `Default`               | Color3    |
| `Texture Coordinates`   | Vector2f  |
| `UV Tiling`             | Vector2f  |
| `UV Offset`             | Vector2f  |
| `Real World Image Size` | Vector2f  |
| `Real World Tile Size`  | Vector2f  |
| `Filter Type`           | String    |

| Output | Type   |
|--------|--------|
| `Out`  | Color3 |

| Input                   | Type      |
|-------------------------|-----------|
| `File`                  | AssetPath |
| `Default`               | Vector3f  |
| `Texture Coordinates`   | Vector2f  |
| `UV Tiling`             | Vector2f  |
| `UV Offset`             | Vector2f  |
| `Real World Image Size` | Vector2f  |
| `Real World Tile Size`  | Vector2f  |
| `Filter Type`           | String    |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3f |

## Parameter descriptions

`File`  
The image file to use for the texture.

`Default`  
A default value to use if the ​file​ reference fails to resolve.

`Texture Coordinates`  
The 2D coordinate at which the data is read in order to map the texture onto a surface. The default is to use the current *UV* coordinates, in which *U* is the horizontal axis and *V* is the vertical axis.

`UV Tiling`  
The tiling rate for the given image along the *U* and *V* axes. The tiling rate is mathematically equivalent to multiplying the incoming texture coordinates by the given vector value. The rate controls how often the `File` repeats in the texture.

`UV Offset`  
The offset for the given image along the U and V axes. The offset is mathematically equivalent to subtracting the given vector value from the incoming texture coordinates.

`Real World Image Size`  
The real-world size represented by the ​file​ image.

`Real World Tile Size`  
The real-world size of a single square `0-1` UV tile.

`Filter Type`  
The type of texture filtering to use.

## Discussion

The Tiled Image material node maps a texture onto a surface with a repeating tiled pattern. It allows you to specify a texture image and control its tiling and real-world size properties. The `UV Tiling` parameter repeats the given file input to produce an image. This image’s size is determined by the `Real World Image Size` parameter. The resulting image is then applied to a single square 0-1 UV tile. The size of this tile is determined by the `Real World Tile Size` parameter. The size of the tile and the size of the image may differ. Therefore, if the image size is larger than the tile it wants to be applied to, the resulting texture will only show part of the image. On the other hand, if the size of the tile is larger than the image, you will see the image repeated in the resulting texture.

Note

While you can create a repeating texture by using the `Real World Image Size` and `Real World Tile Size` parameters, if your only goal is repeating the image, use the `UV Tiling` parameter. Use the size parameters to model real-world dimensions of the image and the surface to which it is applied to.

Below is an example of a simple node graph that uses the Tiled Image node.

If the `UV Tiling` parameter is (2,2) the pattern repeats twice horizontally and twice vertically.

## See Also

### Nodes

Image

A texture referencing a 2D image file.

UV Texture

A MaterialX version of USD UV Texture reader.

Transform 2D

A node that applies an affine transformation to a 2d input.

