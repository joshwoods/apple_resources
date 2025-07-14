

- ShaderGraph
- Data
-  Convert 

ShaderGraph Node

# Convert

Converts a stream from one data type to another.

## Parameter Types

- Convert (float color3f)
- Convert (vector4f vector4h)
- Convert (color3f color4f)
- Convert (vector4f vector3f)
- Convert (float vector4f)
- Convert (vector2f vector2h)
- Convert (integer float)
- Convert (vector3h color3f)
- Convert (vector3f vector3h)
- Convert (float vector2f)
- Convert (vector4f color4f)
- Convert (half color4f)
- Convert (vector3f color3f)
- Convert (vector3f vector4f)
- Convert (vector4h vector4f)
- Convert (bool float)
- Convert (half color3f)
- Convert (float vector3f)
- Convert (color3f vector3f)
- Convert (float color4f)
- Convert (vector3h vector3f)
- Convert (half vector2f)
- Convert (vector2h vector2f)
- Convert (vector2f vector3f)
- Convert (color4f color3f)
- Convert (vector3f vector2f)
- Convert (integer half)
- Convert (color4f vector4f)
- Convert (float half)
- Convert (float integer)
- Convert (half float)
- Convert (half integer)
- Convert (bool half)
- Convert (half vector3f)
- Convert (half vector4f)

| Input | Type  |
|-------|-------|
| `In`  | Float |

| Output | Type   |
|--------|--------|
| `Out`  | Color3 |

| Input | Type     |
|-------|----------|
| `In`  | Vector4f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector4h |

| Input | Type   |
|-------|--------|
| `In`  | Color3 |

| Output | Type   |
|--------|--------|
| `Out`  | Color4 |

| Input | Type     |
|-------|----------|
| `In`  | Vector4f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3f |

| Input | Type  |
|-------|-------|
| `In`  | Float |

| Output | Type     |
|--------|----------|
| `Out`  | Vector4f |

| Input | Type     |
|-------|----------|
| `In`  | Vector2f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector2h |

| Input | Type  |
|-------|-------|
| `In`  | Int32 |

| Output | Type  |
|--------|-------|
| `Out`  | Float |

| Input | Type     |
|-------|----------|
| `In`  | Vector3h |

| Output | Type   |
|--------|--------|
| `Out`  | Color3 |

| Input | Type     |
|-------|----------|
| `In`  | Vector3f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3h |

| Input | Type  |
|-------|-------|
| `In`  | Float |

| Output | Type     |
|--------|----------|
| `Out`  | Vector2f |

| Input | Type     |
|-------|----------|
| `In`  | Vector4f |

| Output | Type   |
|--------|--------|
| `Out`  | Color4 |

| Input | Type |
|-------|------|
| `In`  | Half |

| Output | Type   |
|--------|--------|
| `Out`  | Color4 |

| Input | Type     |
|-------|----------|
| `In`  | Vector3f |

| Output | Type   |
|--------|--------|
| `Out`  | Color3 |

| Input | Type     |
|-------|----------|
| `In`  | Vector3f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector4f |

| Input | Type     |
|-------|----------|
| `In`  | Vector4h |

| Output | Type     |
|--------|----------|
| `Out`  | Vector4f |

| Input | Type |
|-------|------|
| `In`  | Bool |

| Output | Type  |
|--------|-------|
| `Out`  | Float |

| Input | Type |
|-------|------|
| `In`  | Half |

| Output | Type   |
|--------|--------|
| `Out`  | Color3 |

| Input | Type  |
|-------|-------|
| `In`  | Float |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3f |

| Input | Type   |
|-------|--------|
| `In`  | Color3 |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3f |

| Input | Type  |
|-------|-------|
| `In`  | Float |

| Output | Type   |
|--------|--------|
| `Out`  | Color4 |

| Input | Type     |
|-------|----------|
| `In`  | Vector3h |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3f |

| Input | Type |
|-------|------|
| `In`  | Half |

| Output | Type     |
|--------|----------|
| `Out`  | Vector2f |

| Input | Type     |
|-------|----------|
| `In`  | Vector2h |

| Output | Type     |
|--------|----------|
| `Out`  | Vector2f |

| Input | Type     |
|-------|----------|
| `In`  | Vector2f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3f |

| Input | Type   |
|-------|--------|
| `In`  | Color4 |

| Output | Type   |
|--------|--------|
| `Out`  | Color3 |

| Input | Type     |
|-------|----------|
| `In`  | Vector3f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector2f |

| Input | Type  |
|-------|-------|
| `In`  | Int32 |

| Output | Type |
|--------|------|
| `Out`  | Half |

| Input | Type   |
|-------|--------|
| `In`  | Color4 |

| Output | Type     |
|--------|----------|
| `Out`  | Vector4f |

| Input | Type  |
|-------|-------|
| `In`  | Float |

| Output | Type |
|--------|------|
| `Out`  | Half |

| Input | Type  |
|-------|-------|
| `In`  | Float |

| Output | Type  |
|--------|-------|
| `Out`  | Int32 |

| Input | Type |
|-------|------|
| `In`  | Half |

| Output | Type  |
|--------|-------|
| `Out`  | Float |

| Input | Type |
|-------|------|
| `In`  | Half |

| Output | Type  |
|--------|-------|
| `Out`  | Int32 |

| Input | Type |
|-------|------|
| `In`  | Bool |

| Output | Type |
|--------|------|
| `Out`  | Half |

| Input | Type |
|-------|------|
| `In`  | Half |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3f |

| Input | Type |
|-------|------|
| `In`  | Half |

| Output | Type     |
|--------|----------|
| `Out`  | Vector4f |

## Discussion

The Convert node takes data of one type and outputs it in another form. The supported type conversions are shown above with the various convert node types. The convert node handles data types in the following ways:

- When converting a float to a color or vector, the convert node copies the float to all channels of the color or vector.

- When converting a color3 to a color4, the convert node sets the output alpha to `1.0`

- When converting a color4 to a color3, the alpha channel is dropped.

- When converting a boolean or integer to a float, the output is either `1.0` or `0.0`.

- When converting a vector2 to vector3 or a vector3 to a vector4, an additional channel with a value of `1.0` is appended to the input vector.

- When converting a vector4 to a vector3 or a vector3 to a vector2, the last channel is dropped.

## See Also

### Nodes

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

Primvar Reader

A node that provides the ability for shading networks to consume data defined on geometry.

