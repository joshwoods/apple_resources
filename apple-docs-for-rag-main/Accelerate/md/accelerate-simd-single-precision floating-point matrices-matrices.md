

- Accelerate
- simd
-  Single-precision floating-point matrices 

API Collection

# Single-precision floating-point matrices

Perform operations on matrices that contain single-precision floating-point elements.

## Overview

A matrix is a 2D array of values arranged in rows and columns. The simd library provides support for matrices of up to four rows and four columns. It uses a column-major naming convention; for example, a simd_float4x2 is a matrix that contains four columns and two rows.

## Topics

### Matrix structures

struct simd_float2x2

A matrix of two columns and two rows that contains single-precision values.

struct simd_float2x3

A matrix of two columns and three rows that contains single-precision values.

struct simd_float2x4

A matrix of two columns and four rows that contains single-precision values.

struct simd_float3x2

A matrix of three columns and two rows that contains single-precision values.

struct simd_float3x3

A matrix of three columns and three rows that contains single-precision values.

struct simd_float3x4

A matrix of three columns and four rows that contains single-precision values.

struct simd_float4x2

A matrix of four columns and two rows that contains single-precision values.

struct simd_float4x3

A matrix of four columns and three rows that contains single-precision values.

struct simd_float4x4

A matrix of four columns and four rows that contains single-precision values.

## See Also

### Matrices

Working with Matrices

Solve simultaneous equations and transform points in space.

Half-precision floating-point matrices

Perform operations on matrices that contain half-precision floating-point elements.

Double-precision floating-point matrices

Perform operations on matrices that contain double-precision floating-point elements.

