

- Accelerate
-  vSgevv(\_:\_:\_:\_:\_:) Deprecated

Function

# vSgevv(\_:\_:\_:\_:\_:)

Produces the outer product of two vectors and places the results into a matrix.

macOS 10.0–10.14Deprecated

``` source
func vSgevv(
    _ l: Int32,
    _ n: Int32,
    _ A: UnsafePointer,
    _ B: UnsafePointer,
    _ M: UnsafeMutablePointer
)
```

Deprecated

Use cblas_sger on a zero matrix instead

## Parameters 

`l`  

Number of elements in vector `A` and the number of rows in matrix `M`; must be a multiple of 4.

`n`  

Number of elements in vector `B` and the number of columns in matrix `M`; must be a multiple of 4.

`A`  

Vector with `l` elements.

`B`  

Vector with `n` elements.

`M`  

Matrix with `l` rows and `n` columns.

## Discussion

The vectors `A` and `B` are multiplied and the result is stored in matrix `M`, that is, for `0 

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

func vSgetmo(Int32, Int32, UnsafePointer&lt;vFloat>, UnsafeMutablePointer&lt;vFloat>)

Transposes a matrix out of place.

Deprecated

