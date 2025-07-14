

- ShaderGraph
- Data
-  Primvar Reader 

ShaderGraph Node

# Primvar Reader

A node that provides the ability for shading networks to consume data defined on geometry.

## Parameter Types

- Primvar Reader (integer)
- Primvar Reader (vector4f)
- Primvar Reader (vector3f)
- Primvar Reader (bool)
- Primvar Reader (vector2f)
- Primvar Reader (float)

| Input      | Type   |
|------------|--------|
| `Varname`  | String |
| `Fallback` | Int32  |

| Output | Type  |
|--------|-------|
| `Out`  | Int32 |

| Input      | Type     |
|------------|----------|
| `Varname`  | String   |
| `Fallback` | Vector4f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector4f |

| Input      | Type     |
|------------|----------|
| `Varname`  | String   |
| `Fallback` | Vector3f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3f |

| Input      | Type   |
|------------|--------|
| `Varname`  | String |
| `Fallback` | Bool   |

| Output | Type |
|--------|------|
| `Out`  | Bool |

| Input      | Type     |
|------------|----------|
| `Varname`  | String   |
| `Fallback` | Vector2f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector2f |

| Input      | Type   |
|------------|--------|
| `Varname`  | String |
| `Fallback` | Float  |

| Output | Type  |
|--------|-------|
| `Out`  | Float |

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

Separate 2

Outputs each of the channels of a vector2 or integer2 as individual float or integer outputs.

Separate 3

Outputs each of the channels of a color3, vector3, or integer3 as individual float or integer outputs.

Separate 4

Outputs each of the channels of a color4, vector4, or integer4 as individual float or integer outputs.

