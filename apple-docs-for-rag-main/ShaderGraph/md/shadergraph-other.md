

- ShaderGraph
-  Other 

ShaderGraph Node Group

# Other

Perform a wide variety of miscellaneous operations.

## Topics

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

All (RealityKit)

Returns true only if all components of x are true.

Any (RealityKit)

Returns true only if any component of x is true.

Is Finite (RealityKit)

Returns true if the incoming value is finite.

Is Infinite (RealityKit)

Returns true if the incoming value is infinite.

Is Not a Number (RealityKit)

Returns true if the incoming value is a not a number (NaN).

Is Normal (RealityKit)

Test if the incoming value is a normalized floating-point value.

Is Ordered (RealityKit)

Test if arguments are ordered. Returns the result (X == X) && (Y == Y).

Is Unordered (RealityKit)

Test if arguments are unordered. Returns true if X or Y is NaN, otherwise returns false.

Sign Bit (RealityKit)

Tests for sign bit. Returns true if the sign bit is set for the value in X, otherwise returns false.

Select (RealityKit)

Selects B if conditional is true, A if false.

Inverse Hyperbolic Cos

The inverse hyperbolic cosine of the incoming value in radians.

Inverse Hyperbolic Sin

The inverse hyperbolic sine of the incoming value in radians.

Atan

The arctangent of the incoming value in radians.

Inverse Hyperbolic Tan

The hyperbolic arc tangent of the incoming value in radians.

Copy Sign (RealityKit)

Return x with its sign changed to match the sign of y.

Hyperbolic Cos

The hyperbolic cosine of the incoming value in radians.

Cos Pi (RealityKit)

Compute cos(πX).

Exponential 2 (RealityKit)

Exponential Base 2 of X.

Exponential 10 (RealityKit)

Exponential Base 10 of X.

Fortran Difference and Minimum (RealityKit)

Returns X – Y if X \> Y, or +0 if X \

Fused Multiply-Add (RealityKit)

Returns (A \* B) + C.

Max (RealityKit)

Outputs the maximum of two incoming values.

Min (RealityKit)

Outputs the minimum of two incoming values.

Modulo (RealityKit)

Outputs the remaining fraction after dividing the input by a value and subtracting the integer portion.

Fractional-(RealityKit)

Returns the fractional part of a floating point number.

Power Positive (RealityKit)

Computes X to the power of Y, where X is \>= 0

Round Integral (RealityKit)

Rounds X to integral value using round ties to even rounding mode in floating-point format.

Reciprocal Square Root (RealityKit)

Computes inverse square root of X.

Hyperbolic Sin

The hyperbolic sine of the incoming value in radians.

Sin Pi (RealityKit)

Compute sin(πX).

Hyperbolic Tan

The hyperbolic tangent of the incoming value in radians.

Tan Pi (RealityKit)

Compute tan(πX).

Truncate (RealityKit)

Rounds X to integral value using the round-toward-zero rounding mode.

Distance (RealityKit)

Returns the distance between X and Y.

Distance Square (RealityKit)

Returns the square of the distance between X and Y.

Magnitude Square (RealityKit)

Outputs the float magnitude of a vector, squared.

Screen-Space X Partial Derivative (RealityKit)

Returns a high-precision partial derivative of the specified value with respect to the screen space X coordinate.

Screen-Space Y Partial Derivative (RealityKit)

Returns a high-precision partial derivative of the specified value with respect to the screen space Y coordinate.

Absolute Derivatives Sum (RealityKit)

Returns the sum of the absolute derivatives in X and Y using local differencing for p; that is, fabs(dfdx(p)) + fabs(dfdy(p)).

Log 2

The log base 2 of the input.

Log 10

The log base 10 of the input.

Reflection Diffuse (RealityKit)

Diffuse component of reflection.

Reflection Specular (RealityKit)

Specular component of reflection.

### Subscripts

Absolute-(RealityKit)

Outputs the per-channel absolute value of the input.

Absolute-(RealityKit)

Compute absolute value of a floating-point number.

Max3-(RealityKit)

Outputs the maximum of three incoming values.

Max3-(RealityKit)

Outputs the maximum of three incoming values.

Median3-(RealityKit)

Returns the middle value of three incoming values.

Median3-(RealityKit)

Returns the middle value of three incoming values.

Min3-(RealityKit)

Outputs the minimum of three incoming values.

Min3-(RealityKit)

Outputs the minimum of three incoming values.

Multiply-High-(RealityKit)

Computes X \* Y and returns the high half.

Multiply-High-(RealityKit)

Computes X \* Y and returns the high half with Z added to the product.

## See Also

### Node Categories

2D-Procedural

Generate 2D gradients, noise, and other patterns programmatically for your material.

2D-Texture

Load and configure 2D texture files.

3D-Procedural

Generate 3D noise patterns programmatically for your material.

3D-Texture

Project multiple 2D images onto a surface to create a 3D texture.

Adjustment

Modify or convert values, or ranges of values, from one form to another.

Application

Get system values such as the current time or the direction of the up vector.

Compositing

Generate a single output from the combination of multiple data values.

Data

Convert data values to different formats, or manipulate individual elements within a data structure.

Geometric

Access scene geometry while your graph runs.

Logic

Perform Boolean operations and other logical comparisons on data values.

Material

Encapsulate a set of shader graph nodes into a single module.

Math

Perform a wide variety of mathematical and transformative operations on data values.

Organization

Modify the visual flow of data within your graph without changing any values.

Procedural

Add a constant number, vector, matrix, color, string, or other value to your graph.

RealityKit

Add RealityKit surfaces or textures to your material and access and manipulate scene geometry.

