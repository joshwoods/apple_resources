

- Accelerate
-  vSgemm(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:) Deprecated

Function

# vSgemm(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:)

Multiples two general matrices or their transposes, then scales and adds a third.

macOS 10.0–10.14Deprecated

``` source
func vSgemm(
    _ l: Int32,
    _ m: Int32,
    _ n: Int32,
    _ a: UnsafePointer,
    _ forma: CChar,
    _ b: UnsafePointer,
    _ formb: CChar,
    _ c: UnsafeMutablePointer,
    _ alpha: Float,
    _ beta: Float,
    _ matrix: UnsafeMutablePointer
)
```

Deprecated

Use cblas_sgemm instead

## Parameters 

`l`  

Number of rows in matrix `c`; must be a multiple of 4.

`m`  

If `forma` = ‘N’, `m` is the number of columns in matrix `a` ; if `forma` = ‘T’, `m` is the number of rows in matrix `a`. Also, if `formb` = ‘N’, `m` is the number of rows in matrix `b`; if `formb` = ‘T’, `m` is the number of columns in matrix `b`. `m` must be a multiple of 4.

`n`  

Number of columns in matrix `c`; must be a multiple of 4.

`a`  

A matrix with elements of type `float`. If `forma` = ‘N’, the matrix itself is used in the calculation and it has `l` rows and `m` columns. If `forma` = ‘T’, the transpose is used and `a` has `m` rows and `l` columns. Thus the matrix used in the calculation is `l` by `n`.

`forma`  

Selector with a value of ‘N’ or ‘T’.

`b`  

A matrix with elements of type `float`. If `formb` = ‘N’, the matrix itself is used in the calculation and it has `m` rows and `n` columns. If `formb` = ‘T’, the transpose is used and `b` has `n` rows and `m` columns. Thus the matrix used in the calculation is `m` by `n`.

`formb`  

Selector with a value of ‘N’ or ‘T’.

`c`  

An `l` by `n` matrix with elements of type `float`.

`alpha`  

Multiplier for matrix `a`.

`beta`  

Multiplier for matrix `c`.

`matrix`  

Destination matrix with `l` rows and `n` columns.

## Discussion

Matrix `a` (or its transpose) is multiplied by matrix `b` (or its transpose); matrix `c` is multiplied by `beta`, and the result is added to the result of the matrix multiplication; the result is stored in matrix `matrix`

## See Also

### Matrix Operations (from vectorOps.h)

func vSgeadd(Int32, Int32, UnsafePointer&lt;vFloat>, CChar, UnsafePointer&lt;vFloat>, CChar, UnsafeMutablePointer&lt;vFloat>)

Adds two general matrices or their transposes.

Deprecated

func vSgesub(Int32, Int32, UnsafePointer&lt;vFloat>, CChar, UnsafePointer&lt;vFloat>, CChar, UnsafeMutablePointer&lt;vFloat>)

Subtracts two general matrices or their transposes.

Deprecated

func vSgemul(Int32, Int32, Int32, UnsafePointer&lt;vFloat>, CChar, UnsafePointer&lt;vFloat>, CChar, UnsafeMutablePointer&lt;vFloat>)

Multiplies two general matrices or their transposes.

Deprecated

func vSgetmi(Int32, UnsafeMutablePointer&lt;vFloat>)

Transposes a matrix in place.

Deprecated

func vSgetmo(Int32, Int32, UnsafePointer&lt;vFloat>, UnsafeMutablePointer&lt;vFloat>)

Transposes a matrix out of place.

Deprecated

func vSgevv(Int32, Int32, UnsafePointer&lt;vFloat>, UnsafePointer&lt;vFloat>, UnsafeMutablePointer&lt;vFloat>)

Produces the outer product of two vectors and places the results into a matrix.

Deprecated

