

- ShaderGraph
- Data
-  Extract 

ShaderGraph Node

# Extract

Generates a float stream from one channel of a color​N o​r vector​N ​stream.

## Parameter Types

- Extract (color3f)
- Extract (color4f)
- Extract (vector4f)
- Extract (vector3f)
- Extract (vector2f)

| Input   | Type   |
|---------|--------|
| `In`    | Color3 |
| `Index` | Int32  |

| Output | Type  |
|--------|-------|
| `Out`  | Float |

| Input   | Type   |
|---------|--------|
| `In`    | Color4 |
| `Index` | Int32  |

| Output | Type  |
|--------|-------|
| `Out`  | Float |

| Input   | Type     |
|---------|----------|
| `In`    | Vector4f |
| `Index` | Int32    |

| Output | Type  |
|--------|-------|
| `Out`  | Float |

| Input   | Type     |
|---------|----------|
| `In`    | Vector3f |
| `Index` | Int32    |

| Output | Type  |
|--------|-------|
| `Out`  | Float |

| Input   | Type     |
|---------|----------|
| `In`    | Vector2f |
| `Index` | Int32    |

| Output | Type  |
|--------|-------|
| `Out`  | Float |

## Parameter descriptions

`In`  
The input from which to extract a value.

`Index`  
The index of the input from which to extract a value. Default value is `0`.

## Discussion

The Extract node takes its `In` input and always outputs a singular `Float`. The value of the node’s output is the value of number in the `Index` position of `In`. For example, if `In` is equal to a `Vector3` of (10,15,20) and `Index` is `1`, the output is `15`.

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

Separate 2

Outputs each of the channels of a vector2 or integer2 as individual float or integer outputs.

Separate 3

Outputs each of the channels of a color3, vector3, or integer3 as individual float or integer outputs.

Separate 4

Outputs each of the channels of a color4, vector4, or integer4 as individual float or integer outputs.

Primvar Reader

A node that provides the ability for shading networks to consume data defined on geometry.

