

- Accelerate
-  vSrot(\_:\_:\_:\_:\_:) Deprecated

Function

# vSrot(\_:\_:\_:\_:\_:)

Applies planar rotation to a set of n points whose x and y coordinates are contained in two arrays of vectors.

macOS 10.0–10.14Deprecated

``` source
func vSrot(
    _ n: Int32,
    _ x: UnsafeMutablePointer,
    _ y: UnsafeMutablePointer,
    _ c: Float,
    _ s: Float
)
```

Deprecated

Use cblas_srot instead

## Parameters 

`n`  

Number of points to be rotated; must be a multiple of 4.

`x`  

Vector with `n`/4 elements of type `vector float`, representing the x-coordinates of the points.

`y`  

Vector with `n`/4 elements of type `vector float`, representing the y-coordinates of the points.

`c`  

Cosine of the angle of rotation.

`s`  

Sine of the angle of rotation.

## Discussion

The coordinates are modified in place in the vectors in arrays `x` and `y`.

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

func vSscal(Int32, Float, UnsafeMutablePointer&lt;vFloat>)

Scales a vector in place.

Deprecated

func vSswap(Int32, UnsafeMutablePointer&lt;vFloat>, UnsafeMutablePointer&lt;vFloat>)

Interchanges the elements of two vectors.

Deprecated

