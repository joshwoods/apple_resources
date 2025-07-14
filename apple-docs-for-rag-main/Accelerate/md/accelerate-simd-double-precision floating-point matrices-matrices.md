

- Accelerate
- simd
-  Double-precision floating-point matrices 

API Collection

# Double-precision floating-point matrices

Perform operations on matrices that contain double-precision floating-point elements.

## Overview

A matrix is a 2D array of values arranged in rows and columns. The simd library provides support for matrices of up to four rows and four columns. It uses a column-major naming convention; for example, a simd_double4x2 is a matrix that contains four columns and two rows.

## Topics

### Matrix structures

struct simd_double2x2

A matrix of two columns and two rows that contains double-precision values.

struct simd_double2x3

A matrix of two columns and three rows that contains double-precision values.

struct simd_double2x4

A matrix of two columns and four rows that contains double-precision values.

struct simd_double3x2

A matrix of three columns and two rows that contains double-precision values.

struct simd_double3x3

A matrix of three columns and three rows that contains double-precision values.

struct simd_double3x4

A matrix of three columns and four rows that contains double-precision values.

struct simd_double4x2

A matrix of four columns and two rows that contains double-precision values.

struct simd_double4x3

A matrix of four columns and three rows that contains double-precision values.

struct simd_double4x4

A matrix of four columns and four rows that contains double-precision values.

## See Also

### Matrices

Working with Matrices

Solve simultaneous equations and transform points in space.

Half-precision floating-point matrices

Perform operations on matrices that contain half-precision floating-point elements.

Single-precision floating-point matrices

Perform operations on matrices that contain single-precision floating-point elements.

