

- Accelerate
-  vSgetmi(\_:\_:) Deprecated

Function

# vSgetmi(\_:\_:)

Transposes a matrix in place.

macOS 10.0–10.14Deprecated

``` source
func vSgetmi(
    _ size: Int32,
    _ x: UnsafeMutablePointer
)
```

Deprecated

Use appleblas_sgeadd instead

## Parameters 

`size`  

Number of rows and columns in matrix `x`; must be a multiple of 4.

`x`  

Square matrix with `size` rows and `size` columns.

## Discussion

The matrix `x` is transposed in place.

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

func vSgetmo(Int32, Int32, UnsafePointer&lt;vFloat>, UnsafeMutablePointer&lt;vFloat>)

Transposes a matrix out of place.

Deprecated

func vSgevv(Int32, Int32, UnsafePointer&lt;vFloat>, UnsafePointer&lt;vFloat>, UnsafeMutablePointer&lt;vFloat>)

Produces the outer product of two vectors and places the results into a matrix.

Deprecated

