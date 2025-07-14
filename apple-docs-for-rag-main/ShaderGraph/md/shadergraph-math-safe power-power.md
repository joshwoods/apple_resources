

- ShaderGraph
- Math
-  Safe Power 

ShaderGraph Node

# Safe Power

Raises the incoming value to an exponent and assigns the sign of the base to the output.

## Parameter Types

- Safe Power (float)
- Safe Power (vector3f)
- Safe Power (vector2f FA)
- Safe Power (vector3f FA)
- Safe Power (vector4f)
- Safe Power (color4f)
- Safe Power (color4f FA)
- Safe Power (color3f FA)
- Safe Power (vector4f FA)
- Safe Power (vector2f)
- Safe Power (half)
- Safe Power (color3f)

| Input  | Type  |
|--------|-------|
| `In 1` | Float |
| `In 2` | Float |

| Output | Type  |
|--------|-------|
| `Out`  | Float |

| Input  | Type     |
|--------|----------|
| `In 1` | Vector3f |
| `In 2` | Vector3f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3f |

| Input  | Type     |
|--------|----------|
| `In 1` | Vector2f |
| `In 2` | Float    |

| Output | Type     |
|--------|----------|
| `Out`  | Vector2f |

| Input  | Type     |
|--------|----------|
| `In 1` | Vector3f |
| `In 2` | Float    |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3f |

| Input  | Type     |
|--------|----------|
| `In 1` | Vector4f |
| `In 2` | Vector4f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector4f |

| Input  | Type   |
|--------|--------|
| `In 1` | Color4 |
| `In 2` | Color4 |

| Output | Type   |
|--------|--------|
| `Out`  | Color4 |

| Input  | Type   |
|--------|--------|
| `In 1` | Color4 |
| `In 2` | Float  |

| Output | Type   |
|--------|--------|
| `Out`  | Color4 |

| Input  | Type   |
|--------|--------|
| `In 1` | Color3 |
| `In 2` | Float  |

| Output | Type   |
|--------|--------|
| `Out`  | Color3 |

| Input  | Type     |
|--------|----------|
| `In 1` | Vector4f |
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
| `Out`  | Vector2f |

| Input  | Type |
|--------|------|
| `In 1` | Half |
| `In 2` | Half |

| Output | Type |
|--------|------|
| `Out`  | Half |

| Input  | Type   |
|--------|--------|
| `In 1` | Color3 |
| `In 2` | Color3 |

| Output | Type   |
|--------|--------|
| `Out`  | Color3 |

## Discussion

The output of this node is represented by the equation `safepow(x,y) = sign(x) * pow(abs(x), y)`

## See Also

### Nodes

Add

Adds two values.

Subtract

Subtracts two values.

Multiply

Multiplies two values.

Divide

Divides two values.

Modulo

Outputs the remaining fraction after dividing the input by a value and subtracting the integer portion.

Abs

Outputs the per-channel absolute value of the input.

Floor

Outputs the nearest integer value, per-channel, less than or equal to the incoming values.

Ceiling

Outputs the nearest integer value, per-channel, greater than or equal to the incoming values.

Power

Raises the incoming value to an exponent.

Sin

The sine of the incoming value in radians.

Cos

The cosine of the incoming value in radians.

Tan

The tangent of the incoming value in radians.

Asin

The arcsine of the incoming value in radians.

Acos

The arccosine of the incoming value in radians.

Atan2

The arctangent of the expression (iny/inx) in radians.

