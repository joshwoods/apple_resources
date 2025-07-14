

- Accelerate
-  vS64FullMulOdd(\_:\_:) 

Function

# vS64FullMulOdd(\_:\_:)

Signed 64-bit multiplication; results are twice as wide as multiplicands, odd-numbered elements of multiplicand vectors are used. Note the big-endian convention: the leftmost element is element 0.

macOS 10.0+

``` source
func vS64FullMulOdd(
    _ vA: vSInt32,
    _ vB: vSInt32
) -> vSInt32
```

## See Also

### Integer Arithmetic Functions (from vBasicOps.h)

func vU64AddS(vUInt32, vUInt32) -> vUInt32

Unsigned 64-bit addition with saturation (clipping).

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

func vU64SubS(vUInt32, vUInt32) -> vUInt32

Unsigned 64-bit subtraction with saturation (clipping).

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

func vU32HalfMultiply(vUInt32, vUInt32) -> vUInt32

Unsigned 32-bit multiplication; results are same width as multiplicands.

