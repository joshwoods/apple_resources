

- Accelerate
-  vU32Divide(\_:\_:\_:) 

Function

# vU32Divide(\_:\_:\_:)

Unsigned 32-bit division.

macOS 10.0+

``` source
func vU32Divide(
    _ vN: vUInt32,
    _ vD: vUInt32,
    _ vRemainder: UnsafeMutablePointer?
) -> vUInt32
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

