

- ShaderGraph
- 2D-Texture
-  UV Texture 

ShaderGraph Node

# UV Texture

A MaterialX version of USD UV Texture reader.

## Parameter Types

| Input      | Type      |
|------------|-----------|
| `Bias`     | Color4    |
| `Fallback` | Color4    |
| `File`     | AssetPath |
| `Scale`    | Color4    |
| `St`       | Vector2f  |
| `Wrap S`   | String    |
| `Wrap T`   | String    |

| Output  | Type   |
|---------|--------|
| `RGBA`  | Color4 |
| `RGB`   | Color3 |
| `Red`   | Float  |
| `Green` | Float  |
| `Blue`  | Float  |
| `Alpha` | Float  |

## Parameter descriptions

Bias  
The bias the node applys to all components of the texture. The node adds this parameter to the texture after it is multipled by the scale.

Fallback  
The value to use if the texture cannot be read from the file.

File  
The image file to use for the texture.

Scale  
The scale the node applys to all components of the texture. The node multiplies the texture value by this parameter.

St  
The 2D coordinate at which the data is read in order to map the texture onto a surface. This node maps from st to uv image space. The `(0,0)` coordinate in st image space maps to the `(0,0)` coordinate in the `uv` space which represents the lower-left-hand corner. The `(1,1)` coordinate in st image space maps to the `(1,1)` coordinate in `uv` space which represents the upper-right-hand-corner.

Wrap S  
The way that the node will handle *S* values outside of the range of `0-1`.

Wrap T  
The way that the node will handle *T* values outside of the range of `0-1`.

## Output descriptions

RGBA  
The `Color4` output of the texture that contains a red, green, blue, and alpha component.

RGB  
The standard `Color3` output of the texture that contains a red, green, and blue component.

Read  
Only the red component of the texture.

Green  
Only the green component of the texture.

Blue  
Only the blue component of the texture.

Alpha  
Only the alpha component of the texture.

## Discussion

The Wrap parameters for the node tell the node how to handle S and T values outside of the normal range of `0-1`. These inputs take one of four values to determine there behavior.

- black: Texture coordinates outside the normal range return black.

- clamp: Texture coordinates outside the normal range are clamped to the normal range. Any values greater than `1` will be set to `1` and any values less than `0` will be set to `0`

- periodic: Texture coordinates outside the normal range will “wrap around”. This is effectively equivalent to modulo 1 being applied to the coordinates.

## See Also

### Nodes

Image

A texture referencing a 2D image file.

Tiled Image

Samples data from an image with provisions for offsetting and tiling in UV space.

Transform 2D

A node that applies an affine transformation to a 2d input.

