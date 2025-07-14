

- ShaderGraph
- Math
-  Rotate 3D 

ShaderGraph Node

# Rotate 3D

Rotates a Vector3 (Float) about a specified unit axis vector.

## Parameter Types

| Input    | Type     |
|----------|----------|
| `In`     | Vector3f |
| `Amount` | Float    |
| `Axis`   | Vector3f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3f |

## Parameter descriptions

`In`  
The vector to rotate.

`Amount`  
The amount of degrees to rotate the `In` vector. The default value is `0`.

`Axis`  
The unit axis vector that the node rotates the `In` vector around. The default value is `(0, 1, 0)`

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

