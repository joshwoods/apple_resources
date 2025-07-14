

- ShaderGraph
- Other
-  Reciprocal Square Root (RealityKit) 

ShaderGraph Node

# Reciprocal Square Root (RealityKit)

Computes inverse square root of X.

## Parameter Types

- Reciprocal Square Root (half)
- Reciprocal Square Root (vector3h)
- Reciprocal Square Root (vector2h)
- Reciprocal Square Root (vector4h)
- Reciprocal Square Root (float)
- Reciprocal Square Root (vector2f)
- Reciprocal Square Root (vector3f)
- Reciprocal Square Root (vector4f)

| Input | Type |
|-------|------|
| `X`   | Half |

| Output | Type |
|--------|------|
| `Out`  | Half |

| Input | Type     |
|-------|----------|
| `X`   | Vector3h |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3h |

| Input | Type     |
|-------|----------|
| `X`   | Vector2h |

| Output | Type     |
|--------|----------|
| `Out`  | Vector2h |

| Input | Type     |
|-------|----------|
| `X`   | Vector4h |

| Output | Type     |
|--------|----------|
| `Out`  | Vector4h |

| Input | Type  |
|-------|-------|
| `X`   | Float |

| Output | Type  |
|--------|-------|
| `Out`  | Float |

| Input | Type     |
|-------|----------|
| `X`   | Vector2f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector2f |

| Input | Type     |
|-------|----------|
| `X`   | Vector3f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector3f |

| Input | Type     |
|-------|----------|
| `X`   | Vector4f |

| Output | Type     |
|--------|----------|
| `Out`  | Vector4f |

## See Also

### Nodes

Add Saturate (RealityKit)

Returns X + Y and saturates the result.

Count Leading Zeros (RealityKit)

Returns the number of leading 0-bits in X, starting at the most significant bit position.

Count Trailing Zeros (RealityKit)

Returns the count of trailing 0-bits in X, starting at the least significant bit position.

Extract Bits (RealityKit)

Extract bits \[Offset, Offset + Bits - 1\] from X, returning them in the least significant bits of the result.

Integer Average, Rounded Down (RealityKit)

Uses the `hadd` metal instruction to return (x + y) \>\> 1. The intermediate sum does not modulo overflow.

Insert Bits (RealityKit)

Returns the insertion of the Bits least-significant bits of Insert into Base. The result has bits \[Offset, Offset + Bits - 1\] taken from bits \[0, Bits - 1\] of Insert, and all other bits are taken directly from the corresponding bits of Base.

Multiply Add Saturate (RealityKit)

Returns A \* B + C and saturates the result.

Count Non Zeros (RealityKit)

Returns the number of non-zero bits in X.

Reverse Bits (RealityKit)

Returns the reversal of the bits of X. The bit numbered N of the result is taken from bit (Bits – 1) – n of X, where Bits is the total number of bits used to represent X.

Integer Average, Rounded Up (RealityKit)

Uses the `rhadd` metal instruction to return (x + y + 1) \>\> 1. The intermediate sum does not modulo overflow.

Rotate Bits (RealityKit)

For each element in V,the bits are shifted left by the corresponding element in I. Bits shifted off the left side of the element are shifted back in from the right.

Subtract Saturate (RealityKit)

Returns X – Y and saturates the result.

Absolute Diff (RealityKit)

Return \|X - Y\| without modulo overflow.

Multiply Add 24 (RealityKit)

Multiplies two 24-bit integer values X and Y and returns the 32-bit integer result with 32-bit Z value added. X and Y are 32-bit integers but only the low 24 bits perform the multiplication.

Multiply 24 (RealityKit)

Multiplies two 24-bit integer values X and Y and returns the 32-bit integer result. X and Y are 32-bit integers but only the low 24 bits perform the multiplication.

