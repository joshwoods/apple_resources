

- Accelerate
-  vSgemv(\_:\_:\_:\_:\_:\_:\_:\_:) Deprecated

Function

# vSgemv(\_:\_:\_:\_:\_:\_:\_:\_:)

Multiplies a vector by a scalar. Multiplies a matrix by another scalar, then by a second vector, and adds the resulting vector to the first vector. This function can also perform the calculation with the transpose of the original matrix instead of the matrix itself. A selector parameter determines whether the transpose is used.

macOS 10.0–10.14Deprecated

``` source
func vSgemv(
    _ forma: CChar,
    _ m: Int32,
    _ n: Int32,
    _ alpha: Float,
    _ a: UnsafePointer,
    _ x: UnsafePointer,
    _ beta: Float,
    _ y: UnsafeMutablePointer
)
```

Deprecated

Use cblas_sgemv instead

## Parameters 

`forma`  

Selects the variant computation to be performed: ‘T’ causes the transpose of matrix `a` to be used, ‘N’ causes `a` itself to be used.

`m`  

Number of rows in `a`. If `forma` = ‘N’, `m` is the length of vector `y`; if `forma` = ‘T’, `m` is the length of vector `x`; must be a multiple of 4.

`n`  

Number of columns in `a`. If `forma` = ‘N’, `m` is the length of vector `x`; if `forma` = ‘T’, `m` is the length of vector `y`; must be a multiple of 4.

`alpha`  

Scalar multiplier for matrix `a`.

`a`  

`m` by `n` matrix with elements of type `float`.

`x`  

Vector with elements of type `float`.

`beta`  

Scalar multiplier for vector `y`.

`y`  

Destination vector with `n` elements of type `float`.

## Discussion

Vector `y` is multiplied by `beta`. Matrix `a` is multiplied by `alpha`. Then if `forma` = ‘N’, `a` is multiplied by vector `x`; if `forma` = ‘T’, the transpose of `a` is multiplied by `x`. The resulting vector is added to vector `y`, and the results are stored in `y`.

## See Also

### Matrix-Vector Linear Algebra Functions (from vectorOps.h)

func vSgemx(Int32, Int32, Float, UnsafePointer&lt;vFloat>, UnsafePointer&lt;vFloat>, UnsafeMutablePointer&lt;vFloat>)

Multiplies a matrix by a scalar and then by a vector, and adds the resulting vector to a second vector.

Deprecated

func vSgemtx(Int32, Int32, Float, UnsafePointer&lt;vFloat>, UnsafePointer&lt;vFloat>, UnsafeMutablePointer&lt;vFloat>)

Forms the transpose of a matrix, multiplies it by a scalar and then by a vector, and adds the resulting vector to a second vector.

Deprecated

