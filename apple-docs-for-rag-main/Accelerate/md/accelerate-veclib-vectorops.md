

- Accelerate
- vecLib
-  vectorOps 

API Collection

# vectorOps

Perform vector and matrix BLAS functions on arrays of 128-bit vectors.

## Overview

vectorOps.h declares a set of vector and matrix BLAS functions on arrays of 128-bit vectors containing single-precision floating-point values. The arrays can be of any desired length, but the number of `float` elements must be a multiple of 4.

## Topics

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

func vSscal(Int32, Float, UnsafeMutablePointer&lt;vFloat>)

Scales a vector in place.

Deprecated

func vSswap(Int32, UnsafeMutablePointer&lt;vFloat>, UnsafeMutablePointer&lt;vFloat>)

Interchanges the elements of two vectors.

Deprecated

func vSyax(Int32, Float, UnsafePointer&lt;vFloat>, UnsafeMutablePointer&lt;vFloat>)

Multiplies each element of a vector and stores the results in a second vector.

Deprecated

func vSzaxpy(Int32, Float, UnsafePointer&lt;vFloat>, UnsafePointer&lt;vFloat>, UnsafeMutablePointer&lt;vFloat>)

Multiplies a vector by a scalar, adds it to a second vector, and stores the result in a third vector.

Deprecated

### Matrix-Vector Linear Algebra Functions (from vectorOps.h)

func vSgemv(CChar, Int32, Int32, Float, UnsafePointer&lt;vFloat>, UnsafePointer&lt;vFloat>, Float, UnsafeMutablePointer&lt;vFloat>)

Multiplies a vector by a scalar. Multiplies a matrix by another scalar, then by a second vector, and adds the resulting vector to the first vector. This function can also perform the calculation with the transpose of the original matrix instead of the matrix itself. A selector parameter determines whether the transpose is used.

Deprecated

func vSgemx(Int32, Int32, Float, UnsafePointer&lt;vFloat>, UnsafePointer&lt;vFloat>, UnsafeMutablePointer&lt;vFloat>)

Multiplies a matrix by a scalar and then by a vector, and adds the resulting vector to a second vector.

Deprecated

func vSgemtx(Int32, Int32, Float, UnsafePointer&lt;vFloat>, UnsafePointer&lt;vFloat>, UnsafeMutablePointer&lt;vFloat>)

Forms the transpose of a matrix, multiplies it by a scalar and then by a vector, and adds the resulting vector to a second vector.

Deprecated

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

func vSgevv(Int32, Int32, UnsafePointer&lt;vFloat>, UnsafePointer&lt;vFloat>, UnsafeMutablePointer&lt;vFloat>)

Produces the outer product of two vectors and places the results into a matrix.

Deprecated

