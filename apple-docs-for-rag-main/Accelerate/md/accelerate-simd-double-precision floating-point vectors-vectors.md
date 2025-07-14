

- Accelerate
- simd
-  Double-precision floating-point vectors 

API Collection

# Double-precision floating-point vectors

Perform operations on vectors that contain double-precision floating-point elements.

## Overview

The simd library provides many functions in this group, in three variants:

- The default variant—for example, simd_rsqrt(_:)

- The precise variant—for example, simd_precise_rsqrt(_:)

- The fast variant—for example, simd_fast_rsqrt(_:)

The precise variants are accurate to a few units in the last place (ULPs). The fast variants provide greater speed but may have as little as 22 bits of accuracy for double-precision functions.

The compiler flag defines the behavior of the default variant. Ordinarily, the compiler resolves the default variants to their precise counterparts. Set the `-ffast-math` compiler flag to specify that the default variants of the functions resolve to the fast variants.

## Topics

### Vector data types

typealias simd_double1

A vector of one 64-bit floating-point element.

typealias simd_double2

A vector of two 64-bit floating-point elements.

typealias simd_double3

A vector of three 64-bit floating-point elements.

typealias simd_double4

A vector of four 64-bit floating-point elements.

typealias simd_double8

A vector of eight 64-bit floating-point elements.

### Packed vector data types

typealias simd_packed_double2

A packed vector of two 64-bit floating-point elements.

typealias simd_packed_double4

A packed vector of four 64-bit floating-point elements.

typealias simd_packed_double8

A packed vector of eight 64-bit floating-point elements.

## See Also

### Floating-Point Vectors

Working with Vectors

Use vectors to calculate geometric values, calculate dot products and cross products, and interpolate between values.

Half-precision floating-point vectors

Perform operations on vectors that contain half-precision floating-point elements.

Single-precision floating-point vectors

Perform operations on vectors that contain single-precision floating-point elements.

