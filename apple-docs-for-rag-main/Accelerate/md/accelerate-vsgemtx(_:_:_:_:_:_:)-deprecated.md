

- Accelerate
-  vSgemtx(\_:\_:\_:\_:\_:\_:) Deprecated

Function

# vSgemtx(\_:\_:\_:\_:\_:\_:)

Forms the transpose of a matrix, multiplies it by a scalar and then by a vector, and adds the resulting vector to a second vector.

macOS 10.0–10.14Deprecated

``` source
func vSgemtx(
    _ m: Int32,
    _ n: Int32,
    _ alpha: Float,
    _ a: UnsafePointer,
    _ x: UnsafePointer,
    _ y: UnsafeMutablePointer
)
```

Deprecated

Use cblas_sgemv instead

## Parameters 

`m`  

Number of rows in `a`, and the length of vector `y`; must be a multiple of 4.

`n`  

Number of columns in `a`, and the length of vector `x`; must be a multiple of 4.

`alpha`  

Scalar multiplier for matrix `a`.

`a`  

`m` by `n` matrix with elements of type `float`.

`x`  

Vector with elements of type `float`.

`y`  

Destination vector with `n` elements of type `float`.

## Discussion

The transpose of matrix `a` is multiplied by `alpha` and then by vector `x`; the resulting vector is added to vector `y`, and the results are stored in `y`.

## See Also

### Matrix-Vector Linear Algebra Functions (from vectorOps.h)

func vSgemv(CChar, Int32, Int32, Float, UnsafePointer&lt;vFloat>, UnsafePointer&lt;vFloat>, Float, UnsafeMutablePointer&lt;vFloat>)

Multiplies a vector by a scalar. Multiplies a matrix by another scalar, then by a second vector, and adds the resulting vector to the first vector. This function can also perform the calculation with the transpose of the original matrix instead of the matrix itself. A selector parameter determines whether the transpose is used.

Deprecated

func vSgemx(Int32, Int32, Float, UnsafePointer&lt;vFloat>, UnsafePointer&lt;vFloat>, UnsafeMutablePointer&lt;vFloat>)

Multiplies a matrix by a scalar and then by a vector, and adds the resulting vector to a second vector.

Deprecated

