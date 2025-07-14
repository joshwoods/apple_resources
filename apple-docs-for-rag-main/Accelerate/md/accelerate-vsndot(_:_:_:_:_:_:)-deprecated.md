

- Accelerate
-  vSndot(\_:\_:\_:\_:\_:\_:) Deprecated

Function

# vSndot(\_:\_:\_:\_:\_:\_:)

Computes the dot products of n pairs of vectors, accumulating or storing the results in an array of `n` `float` values.

macOS 10.0–10.14Deprecated

``` source
func vSndot(
    _ n: Int32,
    _ m: Int32,
    _ s: UnsafeMutablePointer,
    _ isw: Int32,
    _ x: UnsafePointer,
    _ y: UnsafePointer
)
```

Deprecated

Use cblas_sdot or vDSP_dotpr in a loop instead

## Parameters 

`n`  

Number of dot products to compute, and number of elements in vector `s` ; must be a multiple of 4.

`m`  

Number of elements in the vectors whose dot products are computed; must be a multiple of 4.

`s`  

Destination vector; the `n` dot products are accumulated or stored here.

`isw`  

A key that selects one of the four variants of this function: see Discussion below.

`x`  

A matrix whose rows are `n` floating-point vectors, each containing `m` values.

`y`  

A second matrix whose rows are `n` floating-point vectors, each containing `m` values.

## Discussion

For i = 0 to n-1, the dot product of vectors `x`\[i\] and `y`\[i\] is computed. The dot product is accumulated or stored in `s`\[i\], according to the value of `isw`:

- if `isw` = 1, the dot product is stored in `s`\[i\].

- if `isw` = 2, the dot product is negated and then stored in `s`\[i\].

- if `isw` = 3, the dot product is added to the value in `s`\[i\].

- if `isw` = 4, the dot product is negated and then added to the value in `s`\[i\].

## See Also

### Vector-Scalar Linear Algebra Functions (from vectorOps.h)

func vIsamax(Int32, UnsafePointer&lt;vFloat>) -> Int32

Finds the position of the first vector element having the largest absolute value.

Deprecated

func vIsamin(Int32, UnsafePointer&lt;vFloat>) -> Int32

Finds the position of the first vector element having the smallest absolute value.

Deprecated

func vIsmax(Int32, UnsafePointer&lt;vFloat>) -> Int32

Finds the position of the first vector element having the maximum value.

Deprecated

func vIsmin(Int32, UnsafePointer&lt;vFloat>) -> Int32

Finds the position of the first vector element having the minimum value.

Deprecated

func vSasum(Int32, UnsafePointer&lt;vFloat>) -> Float

Finds the sum of the absolute values of the elements in a vector.

Deprecated

func vSsum(Int32, UnsafePointer&lt;vFloat>) -> Float

Finds the sum of the values of the elements in a vector.

Deprecated

func vSaxpy(Int32, Float, UnsafePointer&lt;vFloat>, UnsafeMutablePointer&lt;vFloat>)

Multiplies a vector by a scalar , adds it to a second vector , and stores the result in the second vector.

Deprecated

func vSnaxpy(Int32, Int32, UnsafePointer&lt;vFloat>, UnsafePointer&lt;vFloat>, UnsafeMutablePointer&lt;vFloat>)

Performs the computation of `vSaxpy` `n` times, using a different multiplier each time.

Deprecated

func vScopy(Int32, UnsafePointer&lt;vFloat>, UnsafeMutablePointer&lt;vFloat>)

Copies one vector to another.

Deprecated

func vSdot(Int32, UnsafePointer&lt;vFloat>, UnsafePointer&lt;vFloat>) -> Float

Computes the dot product of two vectors.

Deprecated

func vSnrm2(Int32, UnsafePointer&lt;vFloat>) -> Float

Finds the Euclidean length of a vector.

Deprecated

func vSnorm2(Int32, UnsafePointer&lt;vFloat>) -> Float

Finds the Euclidean length of a vector.

Deprecated

func vSrot(Int32, UnsafeMutablePointer&lt;vFloat>, UnsafeMutablePointer&lt;vFloat>, Float, Float)

Applies planar rotation to a set of n points whose x and y coordinates are contained in two arrays of vectors.

Deprecated

func vSscal(Int32, Float, UnsafeMutablePointer&lt;vFloat>)

Scales a vector in place.

Deprecated

func vSswap(Int32, UnsafeMutablePointer&lt;vFloat>, UnsafeMutablePointer&lt;vFloat>)

Interchanges the elements of two vectors.

Deprecated

