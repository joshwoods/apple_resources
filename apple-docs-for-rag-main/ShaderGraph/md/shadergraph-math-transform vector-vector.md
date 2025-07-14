

- ShaderGraph
- Math
-  Transform Vector 

ShaderGraph Node

# Transform Vector

Transforms a vector3 from one space to another.

## Parameter Types

| Input       | Type     |
|-------------|----------|
| `In`        | Vector3f |
| `Fromspace` | String   |
| `Tospace`   | String   |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3f |

## Parameter descriptions

`In`  
The normal vector to be transformed.

`Fromspace`  
The space from which to transform the `In` vector.

`Tospace`  
The space to which to transform the `In` vector.

## Discussion

The following spaces are valid values for the `Fromspace` and `Tospace` parameters:

- `model`: The local coordinate space in relation to the model.

- `object`: The coordinate space in relation to the object.

- `world`: The global coordinate in relation to the world as a whole.

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

