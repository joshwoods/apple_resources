

- Accelerate
-  vSnrm2(\_:\_:) Deprecated

Function

# vSnrm2(\_:\_:)

Finds the Euclidean length of a vector.

macOS 10.0–10.14Deprecated

``` source
func vSnrm2(
    _ count: Int32,
    _ x: UnsafePointer
) -> Float
```

Deprecated

Use cblas_snrm2 instead

## Parameters 

`count`  

Number of elements in the vector `x`; must be a multiple of 4.

`x`  

A vector array of `float` values.

## Return Value

The Euclidean length of `x`.

## Discussion

Input is scaled to avoid destructive underflow and overflow.

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

