

- ShaderGraph
- 2D-Procedural
-  Ramp Vertical 

ShaderGraph Node

# Ramp Vertical

A top-to-bottom linear value ramp (gradient) generator.

## Parameter Types

- Ramp Vertical (float)
- Ramp Vertical (vector3h)
- Ramp Vertical (color4f)
- Ramp Vertical (vector2h)
- Ramp Vertical (vector4f)
- Ramp Vertical (half)
- Ramp Vertical (vector2f)
- Ramp Vertical (vector3f)
- Ramp Vertical (vector4h)
- Ramp Vertical (color3f)

| Input                 | Type     |
|-----------------------|----------|
| `Top`                 | Float    |
| `Bottom`              | Float    |
| `Texture Coordinates` | Vector2f |

| Output | Type  |
|--------|-------|
| `Out`  | Float |

| Input                 | Type     |
|-----------------------|----------|
| `Top`                 | Vector3h |
| `Bottom`              | Vector3h |
| `Texture Coordinates` | Vector2f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3h |

| Input                 | Type     |
|-----------------------|----------|
| `Top`                 | Color4   |
| `Bottom`              | Color4   |
| `Texture Coordinates` | Vector2f |

| Output | Type   |
|--------|--------|
| `Out`  | Color4 |

| Input                 | Type     |
|-----------------------|----------|
| `Top`                 | Vector2h |
| `Bottom`              | Vector2h |
| `Texture Coordinates` | Vector2f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector2h |

| Input                 | Type     |
|-----------------------|----------|
| `Top`                 | Vector4f |
| `Bottom`              | Vector4f |
| `Texture Coordinates` | Vector2f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector4f |

| Input                 | Type     |
|-----------------------|----------|
| `Top`                 | Half     |
| `Bottom`              | Half     |
| `Texture Coordinates` | Vector2f |

| Output | Type |
|--------|------|
| `Out`  | Half |

| Input                 | Type     |
|-----------------------|----------|
| `Top`                 | Vector2f |
| `Bottom`              | Vector2f |
| `Texture Coordinates` | Vector2f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector2f |

| Input                 | Type     |
|-----------------------|----------|
| `Top`                 | Vector3f |
| `Bottom`              | Vector3f |
| `Texture Coordinates` | Vector2f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3f |

| Input                 | Type     |
|-----------------------|----------|
| `Top`                 | Vector4h |
| `Bottom`              | Vector4h |
| `Texture Coordinates` | Vector2f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector4h |

| Input                 | Type     |
|-----------------------|----------|
| `Top`                 | Color3   |
| `Bottom`              | Color3   |
| `Texture Coordinates` | Vector2f |

| Output | Type   |
|--------|--------|
| `Out`  | Color3 |

## Parameter Descriptions

`Top`  
The top value of the interpolation.

`Bottom`  
The bottom value of the interpolation.

`Texture coordinates`  
The 2D coordinate at which the data is read in order to map the texture onto a surface. The default is to use the current *UV* coordinates, in which *U* is the horizontal axis and *V* is the vertical axis.

## Discussion

This node uses interpolation to create a vertical ramp or gradient from two values. Any point within the output ramp is a mix of the two values. A given point is more similar to the value that its vertical position is closer to. Below is a an example of a simple node graph that uses Ramp Vertical to create a color gradient.

The image below shows the resulting texture, along with the color values on either side.

## See Also

### Nodes

Ramp Horizontal

A left-to-right linear value ramp (gradient) generator.

Ramp 4 Corners

A four-point linear value ramp (gradient) generator.

Split Horizontal

A left-to-right split matte, split at a specified U value.

Split Vertical

A top-to-bottom split matte, split at a specified V value.

Noise 2D

A 2D Perlin noise generator.

Cellular Noise 2D

A 2D cellular noise generator.

Worley Noise 2D

A 2D Worley noise generator.

