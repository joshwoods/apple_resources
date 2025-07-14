

- Accelerate
-  vU512Divide(\_:\_:\_:\_:) 

Function

# vU512Divide(\_:\_:\_:\_:)

Computes the unsigned 512-bit division.

macOS 10.0+

``` source
func vU512Divide(
    _ numerator: UnsafePointer,
    _ divisor: UnsafePointer,
    _ result: UnsafeMutablePointer,
    _ remainder: UnsafeMutablePointer?
)
```

## Discussion

Important

Apple provides the BLAS and LAPACK libraries under the Accelerate framework to be in line with LAPACK 3.9.1. These new interfaces provide additional functionality, as well as a new ILP64 interface. To use the new interfaces, define `ACCELERATE_NEW_LAPACK` before including the Accelerate or vecLib headers. For ILP64 interfaces, also define `ACCELERATE_LAPACK_ILP64`. For Swift projects, specify `ACCELERATE_NEW_LAPACK=1` and `ACCELERATE_LAPACK_ILP64=1` as preprocessor macros in Xcode build settings.

## See Also

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

