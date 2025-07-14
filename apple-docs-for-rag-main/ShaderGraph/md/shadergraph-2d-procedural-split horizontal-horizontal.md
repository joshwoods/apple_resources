

- ShaderGraph
- 2D-Procedural
-  Split Horizontal 

ShaderGraph Node

# Split Horizontal

A left-to-right split matte, split at a specified U value.

## Parameter Types

- Split Horizontal (float)
- Split Horizontal (color4f)
- Split Horizontal (color3f)
- Split Horizontal (vector2f)
- Split Horizontal (half)
- Split Horizontal (vector3f)
- Split Horizontal (vector4f)

| Input                 | Type     |
|-----------------------|----------|
| `Left`                | Float    |
| `Right`               | Float    |
| `Center`              | Float    |
| `Texture Coordinates` | Vector2f |

| Output | Type  |
|--------|-------|
| `Out`  | Float |

| Input                 | Type     |
|-----------------------|----------|
| `Left`                | Color4   |
| `Right`               | Color4   |
| `Center`              | Float    |
| `Texture Coordinates` | Vector2f |

| Output | Type   |
|--------|--------|
| `Out`  | Color4 |

| Input                 | Type     |
|-----------------------|----------|
| `Left`                | Color3   |
| `Right`               | Color3   |
| `Center`              | Float    |
| `Texture Coordinates` | Vector2f |

| Output | Type   |
|--------|--------|
| `Out`  | Color3 |

| Input                 | Type     |
|-----------------------|----------|
| `Left`                | Vector2f |
| `Right`               | Vector2f |
| `Center`              | Float    |
| `Texture Coordinates` | Vector2f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector2f |

| Input                 | Type     |
|-----------------------|----------|
| `Left`                | Half     |
| `Right`               | Half     |
| `Center`              | Float    |
| `Texture Coordinates` | Vector2f |

| Output | Type |
|--------|------|
| `Out`  | Half |

| Input                 | Type     |
|-----------------------|----------|
| `Left`                | Vector3f |
| `Right`               | Vector3f |
| `Center`              | Float    |
| `Texture Coordinates` | Vector2f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3f |

| Input                 | Type     |
|-----------------------|----------|
| `Left`                | Vector4f |
| `Right`               | Vector4f |
| `Center`              | Float    |
| `Texture Coordinates` | Vector2f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector4f |

## Parameter descriptions

`Left`  
The value of the left side of the split.

`Right`  
The value of the right side of the split.

`Center`  
The *U* value at which the output is split. Everything to the left of this value will be equal to the `Left` input. Everything to the right of this value will be equal to the `Right` input. This parameter can range between 0 and 1.

`Texture Coordinates`  
The 2D coordinate at which the data is read in order to map the texture onto a surface. The default uses the current *UV* coordinates, in which *U* is the horizontal axis and *V* is the vertical axis.

## Discussion

This node creates two distinct regions along the horizontal axis. The value of the `Center` input determines these regions. A value of `0` establishes the center at the leftmost position, causing the output to always be equal to the `Right` input. A value of `1` establishes the center at the right-most position. Below is a an example of a simple node graph that uses Split Horizontal to create a split color.

By editing the center value, the texture can be changed to show a larger left or right region. The image below shows the resulting textures.

## See Also

### Nodes

Ramp Horizontal

A left-to-right linear value ramp (gradient) generator.

Ramp Vertical

A top-to-bottom linear value ramp (gradient) generator.

Ramp 4 Corners

A four-point linear value ramp (gradient) generator.

Split Vertical

A top-to-bottom split matte, split at a specified V value.

Noise 2D

A 2D Perlin noise generator.

Cellular Noise 2D

A 2D cellular noise generator.

Worley Noise 2D

A 2D Worley noise generator.

