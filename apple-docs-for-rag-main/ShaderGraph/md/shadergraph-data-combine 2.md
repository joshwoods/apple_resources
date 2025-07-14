

- ShaderGraph
- Data
-  Combine 2 

ShaderGraph Node

# Combine 2

Combines the channels from two streams into two channels of a single output stream of a compatible type.

## Parameter Types

- Combine 2 (vector2f)
- Combine 2 (integer2)
- Combine 2 (vector4f VF)
- Combine 2 (vector4f VV)
- Combine 2 (color4f CF)
- Combine2 (matrix2x2f)

| Input  | Type  |
|--------|-------|
| `In 1` | Float |
| `In 2` | Float |

| Output | Type     |
|--------|----------|
| `Out`  | Vector2f |

| Input  | Type  |
|--------|-------|
| `In 1` | Int32 |
| `In 2` | Int32 |

| Output | Type     |
|--------|----------|
| `Out`  | Integer2 |

| Input  | Type     |
|--------|----------|
| `In 1` | Vector3f |
| `In 2` | Float    |

| Output | Type     |
|--------|----------|
| `Out`  | Vector4f |

| Input  | Type     |
|--------|----------|
| `In 1` | Vector2f |
| `In 2` | Vector2f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector4f |

| Input  | Type   |
|--------|--------|
| `In 1` | Color3 |
| `In 2` | Float  |

| Output | Type   |
|--------|--------|
| `Out`  | Color4 |

| Input  | Type     |
|--------|----------|
| `In 1` | Vector2f |
| `In 2` | Vector2f |

| Output | Type       |
|--------|------------|
| `Out`  | Matrix2x2f |

## See Also

### Nodes

Convert

Converts a stream from one data type to another.

Swizzle

Performs an arbitrary permutation of the channels of the input stream, returning a new stream of the specified type.

Combine 3

Combines the channels from three streams into three channels of a single output stream of a compatible type.

Combine 4

Combines the channels from four streams into four channels of a single output stream of a compatible type.

Extract

Generates a float stream from one channel of a color​N o​r vector​N ​stream.

Separate 2

Outputs each of the channels of a vector2 or integer2 as individual float or integer outputs.

Separate 3

Outputs each of the channels of a color3, vector3, or integer3 as individual float or integer outputs.

Separate 4

Outputs each of the channels of a color4, vector4, or integer4 as individual float or integer outputs.

Primvar Reader

A node that provides the ability for shading networks to consume data defined on geometry.

