

- Accelerate
-  vSscal(\_:\_:\_:) Deprecated

Function

# vSscal(\_:\_:\_:)

Scales a vector in place.

macOS 10.0–10.14Deprecated

``` source
func vSscal(
    _ n: Int32,
    _ alpha: Float,
    _ x: UnsafeMutablePointer
)
```

Deprecated

Use cblas_sscal instead

## Parameters 

`n`  

Number of elements in vector `x`; must be a multiple of 4.

`alpha`  

Scaling factor.

`x`  

Vector with `n` elements of type `float`.

## Discussion

Each element of vector `x` is multiplied in place by `alpha`.

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

func vSndot(Int32, Int32, UnsafeMutablePointer&lt;Float>, Int32, UnsafePointer&lt;vFloat>, UnsafePointer&lt;vFloat>)

Computes the dot products of n pairs of vectors, accumulating or storing the results in an array of `n` `float` values.

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

func vSswap(Int32, UnsafeMutablePointer&lt;vFloat>, UnsafeMutablePointer&lt;vFloat>)

Interchanges the elements of two vectors.

Deprecated

