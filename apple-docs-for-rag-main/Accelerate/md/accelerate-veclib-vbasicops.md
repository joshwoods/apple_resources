

- Accelerate
- vecLib
-  vBasicOps 

API Collection

# vBasicOps

Perform basic arithmetic and logical functions on 128-bit vectors.

## Overview

vBasicOps.h declares a set of basic arithmetic and logical functions on 128-bit vectors, using the integer types from vecLibTypes.h.

The function names begin with “v,” followed by a mnemonic for the type of operation, e.g. “S” or “U” for signed or unsigned, then the width of the operation, then the name of the operation. For example, `vS8Divide` performs division of signed 8-bit values packed into 128-bit vectors.

## Topics

### Shift and Rotate Functions (from vBasicOps.h)

func vLL128Shift(vUInt32, vUInt8) -> vUInt32

128-bit logical left shift.

func vLR128Shift(vUInt32, vUInt8) -> vUInt32

128-bit logical right shift.

func vLL64Shift(vUInt32, vUInt8) -> vUInt32

64-bit logical left shift.

func vLL64Shift2(vUInt32, vUInt8) -> vUInt32

64-bit logical left shift with two shift factors.

func vLR64Shift(vUInt32, vUInt8) -> vUInt32

64-bit logical right shift.

func vLR64Shift2(vUInt32, vUInt8) -> vUInt32

64-bit logical right shift with two shift factors.

func vA64Shift(vUInt32, vUInt8) -> vUInt32

64-bit arithmetic (signed) shift.

func vA64Shift2(vUInt32, vUInt8) -> vUInt32

64-bit arithmetic (signed) shift with two shift factors.

func vA128Shift(vUInt32, vUInt8) -> vUInt32

128-bit arithmetic (signed) shift.

func vL64Rotate(vUInt32, vUInt8) -> vUInt32

64-bit left rotate.

func vR64Rotate(vUInt32, vUInt8) -> vUInt32

64-bit right rotate.

func vL64Rotate2(vUInt32, vUInt8) -> vUInt32

64-bit left rotate with two rotation factors.

func vR64Rotate2(vUInt32, vUInt8) -> vUInt32

64-bit right rotate with two rotation factors.

func vL128Rotate(vUInt32, vUInt8) -> vUInt32

128-bit left rotate.

func vR128Rotate(vUInt32, vUInt8) -> vUInt32

128-bit right rotate.

### Integer Arithmetic Functions (from vBasicOps.h)

vU64Add

Unsigned 64-bit addition (modular arithmetic).

func vU64AddS(vUInt32, vUInt32) -> vUInt32

Unsigned 64-bit addition with saturation (clipping).

vS64Add

Signed 64-bit addition (modular arithmetic).

func vS64AddS(vSInt32, vSInt32) -> vSInt32

Signed 64-bit addition with saturation (clipping).

func vU128Add(vUInt32, vUInt32) -> vUInt32

Unsigned 128-bit addition (modular arithmetic).

func vU128AddS(vUInt32, vUInt32) -> vUInt32

Unsigned 128-bit addition with saturation (clipping).

func vS128Add(vSInt32, vSInt32) -> vSInt32

Signed 128-bit addition (modular arithmetic).

func vS128AddS(vSInt32, vSInt32) -> vSInt32

Signed 128-bit addition with saturation (clipping).

vU64Sub

Unsigned 64-bit subtraction (modular arithmetic).

func vU64SubS(vUInt32, vUInt32) -> vUInt32

Unsigned 64-bit subtraction with saturation (clipping).

vS64Sub

Signed 64-bit subtraction (modular arithmetic).

func vS64SubS(vSInt32, vSInt32) -> vSInt32

Signed 64-bit subtraction with saturation (clipping).

func vU128Sub(vUInt32, vUInt32) -> vUInt32

Unsigned 128-bit subtraction (modular arithmetic).

func vU128SubS(vUInt32, vUInt32) -> vUInt32

Unsigned 128-bit subtraction with saturation (clipping).

func vS128Sub(vSInt32, vSInt32) -> vSInt32

Signed 128-bit subtraction (modular arithmetic).

func vS128SubS(vSInt32, vSInt32) -> vSInt32

Signed 128-bit subtraction with saturation (clipping).

func vU8HalfMultiply(vUInt8, vUInt8) -> vUInt8

Unsigned 8-bit multiplication; results are same width as multiplicands.

func vS8HalfMultiply(vSInt8, vSInt8) -> vSInt8

Signed 8-bit multiplication; results are same width as multiplicands.

vU16HalfMultiply

Unsigned 16-bit multiplication; results are same width as multiplicands.

vS16HalfMultiply

Signed 16-bit multiplication; results are same width as multiplicands.

func vU32HalfMultiply(vUInt32, vUInt32) -> vUInt32

Unsigned 32-bit multiplication; results are same width as multiplicands.

func vS32HalfMultiply(vSInt32, vSInt32) -> vSInt32

Signed 32-bit multiplication; results are same width as multiplicands.

func vU64HalfMultiply(vUInt32, vUInt32) -> vUInt32

Unsigned 64-bit multiplication; results are same width as multiplicands.

func vS64HalfMultiply(vSInt32, vSInt32) -> vSInt32

Signed 64-bit multiplication; results are same width as multiplicands.

func vU128HalfMultiply(vUInt32, vUInt32) -> vUInt32

Unsigned 128-bit multiplication; results are same width as multiplicands.

func vS128HalfMultiply(vSInt32, vSInt32) -> vSInt32

Signed 128-bit multiplication; results are same width as multiplicands.

func vU32FullMulEven(vUInt32, vUInt32) -> vUInt32

Unsigned 32-bit multiplication; results are twice as wide as multiplicands, even-numbered elements of multiplicand vectors are used. Note the big-endian convention: the leftmost element is element 0.

func vU32FullMulOdd(vUInt32, vUInt32) -> vUInt32

Unsigned 32-bit multiplication; results are twice as wide as multiplicands, odd-numbered elements of multiplicand vectors are used. Note the big-endian convention: the leftmost element is element 0.

func vS32FullMulEven(vSInt32, vSInt32) -> vSInt32

Signed 32-bit multiplication; results are twice as wide as multiplicands, even-numbered elements of multiplicand vectors are used. Note the big-endian convention: the leftmost element is element 0.

func vS32FullMulOdd(vSInt32, vSInt32) -> vSInt32

Signed 32-bit multiplication; results are twice as wide as multiplicands, odd-numbered elements of multiplicand vectors are used. Note the big-endian convention: the leftmost element is element 0.

func vU64FullMulEven(vUInt32, vUInt32) -> vUInt32

Unsigned 64-bit multiplication; results are twice as wide as multiplicands, even-numbered elements of multiplicand vectors are used. Note the big-endian convention: the leftmost element is element 0.

func vU64FullMulOdd(vUInt32, vUInt32) -> vUInt32

Unsigned 64-bit multiplication; results are twice as wide as multiplicands, odd-numbered elements of multiplicand vectors are used. Note the big-endian convention: the leftmost element is element 0.

func vS64FullMulEven(vSInt32, vSInt32) -> vSInt32

Signed 64-bit multiplication; results are twice as wide as multiplicands, even-numbered elements of multiplicand vectors are used. Note the big-endian convention: the leftmost element is element 0.

func vS64FullMulOdd(vSInt32, vSInt32) -> vSInt32

Signed 64-bit multiplication; results are twice as wide as multiplicands, odd-numbered elements of multiplicand vectors are used. Note the big-endian convention: the leftmost element is element 0.

func vU8Divide(vUInt8, vUInt8, UnsafeMutablePointer&lt;vUInt8>?) -> vUInt8

Unsigned 8-bit division.

func vS8Divide(vSInt8, vSInt8, UnsafeMutablePointer&lt;vSInt8>?) -> vSInt8

Signed 8-bit division.

func vU16Divide(vUInt16, vUInt16, UnsafeMutablePointer&lt;vUInt16>?) -> vUInt16

Unsigned 16-bit division.

func vS16Divide(vSInt16, vSInt16, UnsafeMutablePointer&lt;vSInt16>?) -> vSInt16

Signed 16-bit division.

func vU32Divide(vUInt32, vUInt32, UnsafeMutablePointer&lt;vUInt32>?) -> vUInt32

Unsigned 32-bit division.

func vS32Divide(vSInt32, vSInt32, UnsafeMutablePointer&lt;vSInt32>?) -> vSInt32

Signed 32-bit division.

func vU64Divide(vUInt32, vUInt32, UnsafeMutablePointer&lt;vUInt32>?) -> vUInt32

Unsigned 64-bit division.

func vS64Divide(vSInt32, vSInt32, UnsafeMutablePointer&lt;vSInt32>?) -> vSInt32

Signed 64-bit division.

func vU128Divide(vUInt32, vUInt32, UnsafeMutablePointer&lt;vUInt32>?) -> vUInt32

Unsigned 128-bit division.

func vS128Divide(vSInt32, vSInt32, UnsafeMutablePointer&lt;vSInt32>?) -> vSInt32

Signed 128-bit division.

