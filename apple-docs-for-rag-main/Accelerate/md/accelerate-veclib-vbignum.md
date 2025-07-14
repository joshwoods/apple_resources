

- Accelerate
- vecLib
-  vBigNum 

API Collection

# vBigNum

Perform arithmetic and logical functions on large integers.

## Overview

The vBigNum module provides arithmetic and logical operations on large integers with lengths of 128, 256, 512, or 1024 bits.

vBigNum includes data types that represent large integer quantities, such as vS512, which defines a 512-bit signed integer. The function names begin with the data type, followed by the name of the operation. For example, vS512Add(_:_:_:) performs the addition of two 512-bit signed integers.

## Topics

### Shifting and rotating large integers

func vLL256Shift(UnsafePointer&lt;vU256>, UInt32, UnsafeMutablePointer&lt;vU256>)

256-bit logical left shift.

func vLR256Shift(UnsafePointer&lt;vU256>, UInt32, UnsafeMutablePointer&lt;vU256>)

256-bit logical right shift.

func vA256Shift(UnsafePointer&lt;vS256>, UInt32, UnsafeMutablePointer&lt;vS256>)

256-bit arithmetic shift.

func vLL512Shift(UnsafePointer&lt;vU512>, UInt32, UnsafeMutablePointer&lt;vU512>)

512-bit logical left shift.

func vLR512Shift(UnsafePointer&lt;vU512>, UInt32, UnsafeMutablePointer&lt;vU512>)

512-bit logical right shift .

func vA512Shift(UnsafePointer&lt;vS512>, UInt32, UnsafeMutablePointer&lt;vS512>)

512-bit arithmetic shift.

func vLL1024Shift(UnsafePointer&lt;vU1024>, UInt32, UnsafeMutablePointer&lt;vU1024>)

1024-bit logical left shift.

func vLR1024Shift(UnsafePointer&lt;vU1024>, UInt32, UnsafeMutablePointer&lt;vU1024>)

1024-bit logical right shift .

func vA1024Shift(UnsafePointer&lt;vS1024>, UInt32, UnsafeMutablePointer&lt;vS1024>)

1024-bit arithmetic shift.

func vL256Rotate(UnsafePointer&lt;vU256>, UInt32, UnsafeMutablePointer&lt;vU256>)

256-bit left rotate.

func vR256Rotate(UnsafePointer&lt;vU256>, UInt32, UnsafeMutablePointer&lt;vU256>)

256-bit right rotate.

func vL512Rotate(UnsafePointer&lt;vU512>, UInt32, UnsafeMutablePointer&lt;vU512>)

512-bit left rotate.

func vR512Rotate(UnsafePointer&lt;vU512>, UInt32, UnsafeMutablePointer&lt;vU512>)

512-bit right rotate.

func vL1024Rotate(UnsafePointer&lt;vU1024>, UInt32, UnsafeMutablePointer&lt;vU1024>)

1024-bit left rotate.

func vR1024Rotate(UnsafePointer&lt;vU1024>, UInt32, UnsafeMutablePointer&lt;vU1024>)

1024-bit right rotate.

### Performing arithmetic operations on large integers

func vU256Add(UnsafePointer&lt;vU256>, UnsafePointer&lt;vU256>, UnsafeMutablePointer&lt;vU256>)

Unsigned 256-bit addition (modular arithmetic).

func vU256AddS(UnsafePointer&lt;vU256>, UnsafePointer&lt;vU256>, UnsafeMutablePointer&lt;vU256>)

Unsigned 256-bit addition with saturation (clipping).

func vS256Add(UnsafePointer&lt;vS256>, UnsafePointer&lt;vS256>, UnsafeMutablePointer&lt;vS256>)

Signed 256-bit addition (modular arithmetic).

func vS256AddS(UnsafePointer&lt;vS256>, UnsafePointer&lt;vS256>, UnsafeMutablePointer&lt;vS256>)

Signed 256-bit addition with saturation (clipping).

func vU512Add(UnsafePointer&lt;vU512>, UnsafePointer&lt;vU512>, UnsafeMutablePointer&lt;vU512>)

Unsigned 512-bit addition (modular arithmetic).

func vU512AddS(UnsafePointer&lt;vU512>, UnsafePointer&lt;vU512>, UnsafeMutablePointer&lt;vU512>)

Unsigned 512-bit addition with saturation (clipping).

func vS512Add(UnsafePointer&lt;vS512>, UnsafePointer&lt;vS512>, UnsafeMutablePointer&lt;vS512>)

Signed 512-bit addition (modular arithmetic).

func vS512AddS(UnsafePointer&lt;vS512>, UnsafePointer&lt;vS512>, UnsafeMutablePointer&lt;vS512>)

Signed 512-bit addition with saturation (clipping).

func vU1024Add(UnsafePointer&lt;vU1024>, UnsafePointer&lt;vU1024>, UnsafeMutablePointer&lt;vU1024>)

Unsigned 1024-bit addition (modular arithmetic).

func vU1024AddS(UnsafePointer&lt;vU1024>, UnsafePointer&lt;vU1024>, UnsafeMutablePointer&lt;vU1024>)

Unsigned 1024-bit addition with saturation (clipping).

func vS1024Add(UnsafePointer&lt;vS1024>, UnsafePointer&lt;vS1024>, UnsafeMutablePointer&lt;vS1024>)

Signed 1024-bit addition (modular arithmetic).

func vS1024AddS(UnsafePointer&lt;vS1024>, UnsafePointer&lt;vS1024>, UnsafeMutablePointer&lt;vS1024>)

Signed 1024-bit addition with saturation (clipping).

func vU256Sub(UnsafePointer&lt;vU256>, UnsafePointer&lt;vU256>, UnsafeMutablePointer&lt;vU256>)

Unsigned 256-bit subtraction (modular arithmetic).

func vU256SubS(UnsafePointer&lt;vU256>, UnsafePointer&lt;vU256>, UnsafeMutablePointer&lt;vU256>)

Unsigned 256-bit subtraction with saturation (clipping).

func vS256Sub(UnsafePointer&lt;vS256>, UnsafePointer&lt;vS256>, UnsafeMutablePointer&lt;vS256>)

Signed 256-bit subtraction (modular arithmetic).

func vS256SubS(UnsafePointer&lt;vS256>, UnsafePointer&lt;vS256>, UnsafeMutablePointer&lt;vS256>)

Signed 256-bit subtraction with saturation (clipping).

func vU512Sub(UnsafePointer&lt;vU512>, UnsafePointer&lt;vU512>, UnsafeMutablePointer&lt;vU512>)

Unsigned 512-bit subtraction (modular arithmetic).

func vU512SubS(UnsafePointer&lt;vU512>, UnsafePointer&lt;vU512>, UnsafeMutablePointer&lt;vU512>)

Unsigned 512-bit subtraction with saturation (clipping).

func vS512Sub(UnsafePointer&lt;vS512>, UnsafePointer&lt;vS512>, UnsafeMutablePointer&lt;vS512>)

Signed 512-bit subtraction (modular arithmetic).

func vS512SubS(UnsafePointer&lt;vS512>, UnsafePointer&lt;vS512>, UnsafeMutablePointer&lt;vS512>)

Signed 512-bit subtraction with saturation (clipping).

func vU1024Sub(UnsafePointer&lt;vU1024>, UnsafePointer&lt;vU1024>, UnsafeMutablePointer&lt;vU1024>)

Unsigned 1024-bit subtraction (modular arithmetic).

func vU1024SubS(UnsafePointer&lt;vU1024>, UnsafePointer&lt;vU1024>, UnsafeMutablePointer&lt;vU1024>)

Unsigned 1024-bit subtraction with saturation (clipping).

func vS1024Sub(UnsafePointer&lt;vS1024>, UnsafePointer&lt;vS1024>, UnsafeMutablePointer&lt;vS1024>)

Signed 1024-bit subtraction (modular arithmetic).

func vS1024SubS(UnsafePointer&lt;vS1024>, UnsafePointer&lt;vS1024>, UnsafeMutablePointer&lt;vS1024>)

Signed 1024-bit subtraction with saturation (clipping).

func vU64Neg(vUInt32) -> vUInt32

Unsigned 64-bit negation.

func vU128Neg(vUInt32) -> vUInt32

Unsigned 128-bit negation.

func vU256Neg(UnsafePointer&lt;vU256>, UnsafeMutablePointer&lt;vU256>)

Unsigned 256-bit negation.

func vS64Neg(vSInt32) -> vSInt32

Signed 64-bit negation.

func vS128Neg(vSInt32) -> vSInt32

Signed 128-bit negation.

func vS256Neg(UnsafePointer&lt;vS256>, UnsafeMutablePointer&lt;vS256>)

Signed 256-bit negation.

func vU512Neg(UnsafePointer&lt;vU512>, UnsafeMutablePointer&lt;vU512>)

Unsigned 512-bit negation.

func vS512Neg(UnsafePointer&lt;vS512>, UnsafeMutablePointer&lt;vS512>)

Signed 512-bit negation.

func vU1024Neg(UnsafePointer&lt;vU1024>, UnsafeMutablePointer&lt;vU1024>)

Unsigned 1024-bit negation.

func vS1024Neg(UnsafePointer&lt;vS1024>, UnsafeMutablePointer&lt;vS1024>)

Signed 1024-bit negation.

func vU256Mod(UnsafePointer&lt;vU256>, UnsafePointer&lt;vU256>, UnsafeMutablePointer&lt;vU256>)

Unsigned 256-bit mod.

func vS256Mod(UnsafePointer&lt;vS256>, UnsafePointer&lt;vS256>, UnsafeMutablePointer&lt;vS256>)

Signed 256-bit mod.

func vU512Mod(UnsafePointer&lt;vU512>, UnsafePointer&lt;vU512>, UnsafeMutablePointer&lt;vU512>)

Unsigned 512-bit mod.

func vS512Mod(UnsafePointer&lt;vS512>, UnsafePointer&lt;vS512>, UnsafeMutablePointer&lt;vS512>)

Signed 512-bit mod.

func vU1024Mod(UnsafePointer&lt;vU1024>, UnsafePointer&lt;vU1024>, UnsafeMutablePointer&lt;vU1024>)

Unsigned 1024-bit mod.

func vS1024Mod(UnsafePointer&lt;vS1024>, UnsafePointer&lt;vS1024>, UnsafeMutablePointer&lt;vS1024>)

Signed 256-bit Mod.

func vU256HalfMultiply(UnsafePointer&lt;vU256>, UnsafePointer&lt;vU256>, UnsafeMutablePointer&lt;vU256>)

Unsigned 256-bit multiplication; result is the same width as multiplicands.

func vS256HalfMultiply(UnsafePointer&lt;vS256>, UnsafePointer&lt;vS256>, UnsafeMutablePointer&lt;vS256>)

Signed 256-bit multiplication; result is the same width as multiplicands.

func vU512HalfMultiply(UnsafePointer&lt;vU512>, UnsafePointer&lt;vU512>, UnsafeMutablePointer&lt;vU512>)

Unsigned 512-bit multiplication; result is the same width as multiplicands.

func vS512HalfMultiply(UnsafePointer&lt;vS512>, UnsafePointer&lt;vS512>, UnsafeMutablePointer&lt;vS512>)

Signed 512-bit multiplication; result is the same width as multiplicands.

func vU1024HalfMultiply(UnsafePointer&lt;vU1024>, UnsafePointer&lt;vU1024>, UnsafeMutablePointer&lt;vU1024>)

Unsigned 1024-bit multiplication; result is the same width as multiplicands.

func vS1024HalfMultiply(UnsafePointer&lt;vS1024>, UnsafePointer&lt;vS1024>, UnsafeMutablePointer&lt;vS1024>)

Signed 1024-bit multiplication; result is the same width as multiplicands.

func vU128FullMultiply(UnsafePointer&lt;vU128>, UnsafePointer&lt;vU128>, UnsafeMutablePointer&lt;vU256>)

Unsigned 128-bit multiplication; result is twice as wide as multiplicands.

func vS128FullMultiply(UnsafePointer&lt;vS128>, UnsafePointer&lt;vS128>, UnsafeMutablePointer&lt;vS256>)

Signed 128-bit multiplication; result is twice as wide as multiplicands.

func vU256FullMultiply(UnsafePointer&lt;vU256>, UnsafePointer&lt;vU256>, UnsafeMutablePointer&lt;vU512>)

Unsigned 256-bit multiplication; result is twice as wide as multiplicands.

func vS256FullMultiply(UnsafePointer&lt;vS256>, UnsafePointer&lt;vS256>, UnsafeMutablePointer&lt;vS512>)

Signed 256-bit multiplication; result is twice as wide as multiplicands.

func vU512FullMultiply(UnsafePointer&lt;vU512>, UnsafePointer&lt;vU512>, UnsafeMutablePointer&lt;vU1024>)

Unsigned 512-bit multiplication; result is twice as wide as multiplicands.

func vS512FullMultiply(UnsafePointer&lt;vS512>, UnsafePointer&lt;vS512>, UnsafeMutablePointer&lt;vS1024>)

Signed 512-bit multiplication; result is twice as wide as multiplicands.

func vU256Divide(UnsafePointer&lt;vU256>, UnsafePointer&lt;vU256>, UnsafeMutablePointer&lt;vU256>, UnsafeMutablePointer&lt;vU256>?)

Unsigned 256-bit division.

func vS256Divide(UnsafePointer&lt;vS256>, UnsafePointer&lt;vS256>, UnsafeMutablePointer&lt;vS256>, UnsafeMutablePointer&lt;vS256>?)

Computes the signed 256-bit division.

func vU512Divide(UnsafePointer&lt;vU512>, UnsafePointer&lt;vU512>, UnsafeMutablePointer&lt;vU512>, UnsafeMutablePointer&lt;vU512>?)

Computes the unsigned 512-bit division.

func vS512Divide(UnsafePointer&lt;vS512>, UnsafePointer&lt;vS512>, UnsafeMutablePointer&lt;vS512>, UnsafeMutablePointer&lt;vS512>?)

Signed 512-bit division.

func vU1024Divide(UnsafePointer&lt;vU1024>, UnsafePointer&lt;vU1024>, UnsafeMutablePointer&lt;vU1024>, UnsafeMutablePointer&lt;vU1024>?)

Unsigned 1024-bit division.

func vS1024Divide(UnsafePointer&lt;vS1024>, UnsafePointer&lt;vS1024>, UnsafeMutablePointer&lt;vS1024>, UnsafeMutablePointer&lt;vS1024>?)

Signed 1024-bit division.

### Data types

struct vU128

A union containing one `vUInt32` vector or four 32-bit integers, representing a 128-bit unsigned integer.

struct vS128

A union containing one `vSInt32` vector or four 32-bit integers, representing a 128-bit signed integer.

struct vU256

A union containing an array or structure of two `vUInt32` vectors or eight 32-bit integers, representing a 256-bit unsigned integer.

struct vS256

A union containing an array or structure of two `vUInt32` vectors or eight 32-bit integers, representing a 256-bit signed integer.

struct vU512

A union containing an array or structure of four `vUInt32` vectors or sixteen 32-bit integers, representing a 256-bit unsigned integer.

struct vS512

A union containing an array or structure of four `vUInt32` vectors or sixteen 32-bit integers, representing a 256-bit signed integer.

struct vU1024

A union containing an array or structure of eight `vUInt32` vectors or thirty-two 32-bit integers, representing a 1024-bit unsigned integer.

struct vS1024

A union containing an array or structure of eight `vUInt32` vectors or thirty-two 32-bit integers, representing a 1024-bit signed integer.

