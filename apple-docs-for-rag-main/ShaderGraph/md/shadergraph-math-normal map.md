

- ShaderGraph
- Math
-  Normal Map 

ShaderGraph Node

# Normal Map

Transforms a normal vector from object or tangent space into world space.

## Parameter Types

- Normal Map
- Normal Map (vector2f Scale)

| Input     | Type     |
|-----------|----------|
| `In`      | Vector3f |
| `Space`   | String   |
| `Scale`   | Float    |
| `Normal`  | Vector3f |
| `Tangent` | Vector3f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3f |

| Input     | Type     |
|-----------|----------|
| `In`      | Vector3f |
| `Space`   | String   |
| `Scale`   | Vector2f |
| `Normal`  | Vector3f |
| `Tangent` | Vector3f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3f |

## Parameter descriptions

`In`  
The input vector to be transformed. The default value is `(0.5, 0.5, 1.0)`.

`Space`  
The space from which the node transforms the normal vector. The value can either be `object` or `tangent`. The default value is `tangent`.

`Scale`  
A scalar multiplier for the input vector before the node transforms it. The default value is `1.0`.

`Normal`  
The surface normal vector. The default value is the current surface normal of world space.

`Tangent`  
The surface tangent vector. The default value is the current tangent vector of world space.

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

