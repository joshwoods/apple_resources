

- ShaderGraph
- Data
-  Separate 2 

ShaderGraph Node

# Separate 2

Outputs each of the channels of a vector2 or integer2 as individual float or integer outputs.

## Parameter Types

- Separate 2 (vector2f)
- Separate 2

| Input | Type     |
|-------|----------|
| `In`  | Vector2f |

| Output | Type  |
|--------|-------|
| `x`    | Float |
| `y`    | Float |

| Input | Type     |
|-------|----------|
| `In`  | Integer2 |

| Output | Type  |
|--------|-------|
| `Outx` | Int32 |
| `Outy` | Int32 |

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

Combine 4

Combines the channels from four streams into four channels of a single output stream of a compatible type.

Extract

Generates a float stream from one channel of a color​N o​r vector​N ​stream.

Separate 3

Outputs each of the channels of a color3, vector3, or integer3 as individual float or integer outputs.

Separate 4

Outputs each of the channels of a color4, vector4, or integer4 as individual float or integer outputs.

Primvar Reader

A node that provides the ability for shading networks to consume data defined on geometry.

