

- ShaderGraph
- Data
-  Combine 4 

ShaderGraph Node

# Combine 4

Combines the channels from four streams into four channels of a single output stream of a compatible type.

## Parameter Types

- Combine 4 (color4f)
- Combine 4 (matrix4x4f)
- Combine 4 (vector4f)
- Combine 4 (integer4)

| Input  | Type  |
|--------|-------|
| `In 1` | Float |
| `In 2` | Float |
| `In 3` | Float |
| `In 4` | Float |

| Output | Type   |
|--------|--------|
| `Out`  | Color4 |

| Input  | Type     |
|--------|----------|
| `In 1` | Vector4f |
| `In 2` | Vector4f |
| `In 3` | Vector4f |
| `In 4` | Vector4f |

| Output | Type       |
|--------|------------|
| `Out`  | Matrix4x4f |

| Input  | Type  |
|--------|-------|
| `In 1` | Float |
| `In 2` | Float |
| `In 3` | Float |
| `In 4` | Float |

| Output | Type     |
|--------|----------|
| `Out`  | Vector4f |

| Input  | Type  |
|--------|-------|
| `In 1` | Int32 |
| `In 2` | Int32 |
| `In 3` | Int32 |
| `In 4` | Int32 |

| Output | Type     |
|--------|----------|
| `Out`  | Integer4 |

## See Also

### Nodes

Convert

Converts a stream from one data type to another.

Swizzle

Performs an arbitrary permutation of the channels of the input stream, returning a new stream of the specified type.

Combine 2

Combines the channels from two streams into two channels of a single output stream of a compatible type.

Combine 3

Combines the channels from three streams into three channels of a single output stream of a compatible type.

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

