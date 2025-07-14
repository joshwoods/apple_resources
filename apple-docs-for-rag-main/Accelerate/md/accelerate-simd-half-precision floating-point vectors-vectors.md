

- Accelerate
- simd
-  Half-precision floating-point vectors 

API Collection

# Half-precision floating-point vectors

Perform operations on vectors that contain half-precision floating-point elements.

## Overview

The simd library provides many functions in this group, in three variants:

- The default variant—for example, simd_rsqrt(_:)

- The precise variant—for example, simd_precise_rsqrt(_:)

- The fast variant—for example, simd_fast_rsqrt(_:)

The precise variants are accurate to a few units in the last place (ULPs). The fast variants provide greater speed but may have as little as 8 bits of accuracy for half-precision functions.

The compiler flag defines the behavior of the default variant. Ordinarily, the compiler resolves the default variants to their precise counterparts. Set the `-ffast-math` compiler flag to specify that the default variants of the functions resolve to the fast variants.

## Topics

### Vector data types

typealias simd_half1

A vector of one 16-bit floating-point element.

typealias simd_half2

A vector of two 16-bit floating-point elements.

typealias simd_half3

A vector of three 16-bit floating-point elements.

typealias simd_half4

A vector of four 16-bit floating-point elements.

typealias simd_half8

A vector of eight 16-bit floating-point elements.

typealias simd_half16

A vector of sixteen 16-bit floating-point elements.

typealias simd_half32

A vector of thirty-two 16-bit floating-point elements.

## See Also

### Floating-Point Vectors

Working with Vectors

Use vectors to calculate geometric values, calculate dot products and cross products, and interpolate between values.

Single-precision floating-point vectors

Perform operations on vectors that contain single-precision floating-point elements.

Double-precision floating-point vectors

Perform operations on vectors that contain double-precision floating-point elements.

