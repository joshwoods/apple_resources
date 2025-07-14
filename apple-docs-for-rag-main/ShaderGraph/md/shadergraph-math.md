

- ShaderGraph
-  Math 

ShaderGraph Node Group

# Math

Perform a wide variety of mathematical and transformative operations on data values.

## Overview

Include math nodes in your graph when you want to perform typical mathematical operations on data values. A wide range of nodes are available, supporting basic arithmetic, trigonometry, logs, exponents, dot and cross products, and more. Some nodes operate on specific data types of values but most operate on a wide range of data types, including numbers, colors, and vectors.

## Topics

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

Square Root

The square root of the incoming value.

Natural Log

The natural log of the input.

Exp

Outputs ‘e’ to the power of the input.

Sign

The per-channel sign of the input value: -1 for negative, +1 for positive, 0 for zero.

Clamp

Clamps the input per-channel to a specified range.

Min

Outputs the minimum of two incoming values.

Max

Outputs the maximum of two incoming values.

Normalize

Outputs a normalized vector.

Magnitude

Outputs the float magnitude of a vector.

Dot Product

Outputs the dot product of two vectors.

Cross Product

Calculates the cross product vector of 2 input vectors.

Transform Point

Transforms a coordinate from one space to another.

Transform Vector

Transforms a vector3 from one space to another.

Transform Normal

Transforms a normal from one space to another.

Transform Matrix

Transforms a vector by a matrix.

Transpose

Outputs the tranpose of a matrix.

Determinant

Outputs the float determinant of a matrix.

Invert Matrix

Outputs the inverse of a matrix.

Rotate 2D

Rotates a Vector2 (Float) about the origin in 2D.

Rotate 3D

Rotates a Vector3 (Float) about a specified unit axis vector.

Place 2D

Transforms UV texture coordinates for 2D texture placement.

Round

Rounds to the nearest integer value, per-channel.

Safe Power

Raises the incoming value to an exponent and assigns the sign of the base to the output.

Normal Map

Transforms a normal vector from object or tangent space into world space.

Fractional (RealityKit)

Returns the fractional part of a floating point number.

One Minus (RealityKit)

Outputs one minus the input

Normal Map Decode

Remaps a normal’s value from \[0,1\] to \[-1,1\] by applying 2x-1.

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

Organization

Modify the visual flow of data within your graph without changing any values.

Procedural

Add a constant number, vector, matrix, color, string, or other value to your graph.

RealityKit

Add RealityKit surfaces or textures to your material and access and manipulate scene geometry.

Surface

Generate a MaterialX preview surface.

