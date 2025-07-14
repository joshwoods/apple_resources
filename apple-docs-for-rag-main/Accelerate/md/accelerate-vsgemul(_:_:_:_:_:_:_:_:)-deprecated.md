

- Accelerate
-  vSgemul(\_:\_:\_:\_:\_:\_:\_:\_:) Deprecated

Function

# vSgemul(\_:\_:\_:\_:\_:\_:\_:\_:)

Multiplies two general matrices or their transposes.

macOS 10.0–10.14Deprecated

``` source
func vSgemul(
    _ l: Int32,
    _ m: Int32,
    _ n: Int32,
    _ a: UnsafePointer,
    _ forma: CChar,
    _ b: UnsafePointer,
    _ formb: CChar,
    _ matrix: UnsafeMutablePointer
)
```

Deprecated

Use cblas_sgemm instead

## Parameters 

`l`  

Number of rows in matrix `matrix`; must be a multiple of 4.

`m`  

If `forma` = ‘N’, `m` is the number of columns in matrix `a` ; if forma = ‘T’, `m` is the number of rows in matrix `a`. Also, if `formb` = ‘N’, `m` is the number of rows in matrix `b`; if formb = ‘T’, `m` is the number of columns in matrix `b`. `m` must be a multiple of 4.

`n`  

Number of columns in the matrix `matrix`; must be a multiple of 4.

`a`  

A matrix with elements of type `float`. If `forma` = ‘N’, the matrix itself is used in the calculation and it has `l` rows and `m` columns. If `forma` = ‘T’, the transpose is used and `a` has `m` rows and `l` columns. Thus the matrix used in the calculation is `l` by `m`.

`forma`  

Selector with a value of ‘N’ or ‘T’.

`b`  

A matrix with elements of type `float`. If `formb` = ‘N’, the matrix itself is used in the calculation and it has `m` rows and `n` columns. If `formb` = ‘T’, the transpose is used and `b` has `n` rows and `m` columns. Thus the matrix used in the calculation is `m` by `n`.

`formb`  

Selector with a value of ‘N’ or ‘T’.

`matrix`  

Destination matrix with `l` rows and `n` columns.

## Discussion

Matrix `a` (or its transpose) is multiplied by matrix `b` (or its transpose); the result is stored in matrix `matrix`.

## See Also

### Matrix Operations (from vectorOps.h)

func vSgeadd(Int32, Int32, UnsafePointer&lt;vFloat>, CChar, UnsafePointer&lt;vFloat>, CChar, UnsafeMutablePointer&lt;vFloat>)

Adds two general matrices or their transposes.

Deprecated

func vSgesub(Int32, Int32, UnsafePointer&lt;vFloat>, CChar, UnsafePointer&lt;vFloat>, CChar, UnsafeMutablePointer&lt;vFloat>)

Subtracts two general matrices or their transposes.

Deprecated

func vSgemm(Int32, Int32, Int32, UnsafePointer&lt;vFloat>, CChar, UnsafePointer&lt;vFloat>, CChar, UnsafeMutablePointer&lt;vFloat>, Float, Float, UnsafeMutablePointer&lt;vFloat>)

Multiples two general matrices or their transposes, then scales and adds a third.

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

