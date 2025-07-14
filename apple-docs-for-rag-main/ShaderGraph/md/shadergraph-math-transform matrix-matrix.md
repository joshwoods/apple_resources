

- ShaderGraph
- Math
-  Transform Matrix 

ShaderGraph Node

# Transform Matrix

Transforms a vector by a matrix.

## Parameter Types

- Transform Matrix (vector2f matrix3x3f)
- Transform Matrix (vector3f)
- Transform Matrix (vector4f)
- Transform Matrix (vector3f matrix4x4f)
- Transform Matrix (vector2f)

| Input | Type       |
|-------|------------|
| `In`  | Vector2f   |
| `Mat` | Matrix3x3f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector2f |

| Input | Type       |
|-------|------------|
| `In`  | Vector3f   |
| `Mat` | Matrix3x3f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3f |

| Input | Type       |
|-------|------------|
| `In`  | Vector4f   |
| `Mat` | Matrix4x4f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector4f |

| Input | Type       |
|-------|------------|
| `In`  | Vector3f   |
| `Mat` | Matrix4x4f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3f |

| Input | Type       |
|-------|------------|
| `In`  | Vector2f   |
| `Mat` | Matrix2x2f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector2f |

## Parameter descriptions

`In`  
The vector to transform. This node appends an addtional component onto the `In` vector with a value of `1.0` to make the vector match the dimensions of the `Mat` matrix. This additional compenent is removed after the transformation completes.

`Mat`  
The matrix by which to transform the `In` vector. The default value is the identity matrix.

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

