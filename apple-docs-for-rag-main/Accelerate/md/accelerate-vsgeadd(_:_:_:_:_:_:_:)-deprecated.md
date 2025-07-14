

- Accelerate
-  vSgeadd(\_:\_:\_:\_:\_:\_:\_:) Deprecated

Function

# vSgeadd(\_:\_:\_:\_:\_:\_:\_:)

Adds two general matrices or their transposes.

macOS 10.0–10.14Deprecated

``` source
func vSgeadd(
    _ height: Int32,
    _ width: Int32,
    _ a: UnsafePointer,
    _ forma: CChar,
    _ b: UnsafePointer,
    _ formb: CChar,
    _ c: UnsafeMutablePointer
)
```

Deprecated

Use appleblas_sgeadd instead

## Parameters 

`height`  

Number of rows in the matrices to be added; must be a multiple of 4.

`width`  

Number of columns in the matrices to be added; must be a multiple of 4.

`a`  

A matrix with elements of type `float`. If `forma` = ‘N’, the matrix itself is used in the calculation and it has `height` rows and `width` columns. If `forma` = ‘T’, the transpose is used and `a` has `width` rows and `height` columns.

`forma`  

Selector with a value of’N’ or ‘T’.

`b`  

A matrix with elements of type `float`. If `formb` = ‘N’, the matrix itself is used in the calculation and it has `height` rows and `width` columns. If `formb` = ‘T’, the transpose is used and `b` has `width` rows and `height` columns.

`formb`  

Selector with a value of ‘N’ or ‘T’.

`c`  

Destination matrix with `height` rows and `width` columns.

## Discussion

Matrix `a` (or its transpose) is added to matrix `b` (or its transpose); the result is stored in mactrix `c`.

## See Also

### Matrix Operations (from vectorOps.h)

func vSgesub(Int32, Int32, UnsafePointer&lt;vFloat>, CChar, UnsafePointer&lt;vFloat>, CChar, UnsafeMutablePointer&lt;vFloat>)

Subtracts two general matrices or their transposes.

Deprecated

func vSgemul(Int32, Int32, Int32, UnsafePointer&lt;vFloat>, CChar, UnsafePointer&lt;vFloat>, CChar, UnsafeMutablePointer&lt;vFloat>)

Multiplies two general matrices or their transposes.

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

