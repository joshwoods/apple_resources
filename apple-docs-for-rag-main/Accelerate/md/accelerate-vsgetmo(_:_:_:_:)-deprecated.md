

- Accelerate
-  vSgetmo(\_:\_:\_:\_:) Deprecated

Function

# vSgetmo(\_:\_:\_:\_:)

Transposes a matrix out of place.

macOS 10.0–10.14Deprecated

``` source
func vSgetmo(
    _ height: Int32,
    _ width: Int32,
    _ x: UnsafePointer,
    _ y: UnsafeMutablePointer
)
```

Deprecated

Use appleblas_sgeadd instead

## Parameters 

`height`  

Number of rows in matrix `x` and number of columns in matrix y; must be a multiple of 4.

`width`  

Number of columns in matrix `x` and number of rows in matrix y; must be a multiple of 4.

`x`  

Matrix with `height` rows and `width` columns.

`y`  

Matrix with `width` rows and `height` columns.

## Discussion

The matrix `x` is transposed into matrix `y`.

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

func vSgemm(Int32, Int32, Int32, UnsafePointer&lt;vFloat>, CChar, UnsafePointer&lt;vFloat>, CChar, UnsafeMutablePointer&lt;vFloat>, Float, Float, UnsafeMutablePointer&lt;vFloat>)

Multiples two general matrices or their transposes, then scales and adds a third.

Deprecated

func vSgetmi(Int32, UnsafeMutablePointer&lt;vFloat>)

Transposes a matrix in place.

Deprecated

func vSgevv(Int32, Int32, UnsafePointer&lt;vFloat>, UnsafePointer&lt;vFloat>, UnsafeMutablePointer&lt;vFloat>)

Produces the outer product of two vectors and places the results into a matrix.

Deprecated

