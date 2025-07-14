

- Accelerate
-  vvcbrtf(\_:\_:\_:) 

Function

# vvcbrtf(\_:\_:\_:)

Calculates the cube root for each element of a vector.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func vvcbrtf(
    _: UnsafeMutablePointer,
    _: UnsafePointer,
    _: UnsafePointer
)
```

### Parameters

y  
(output) Output vector of size `*n`. `y[i]` is set to `cbrt(x[i])`.

x  
(input) Input vector of size `*n`.

n  
(input) The number of elements in the vectors `x` and `y`.

## See Also

### Trigonometric Functions (from vfp.h)

func vsinf(vFloat) -> vFloat

For each vector element, calculates the sine.

func vcosf(vFloat) -> vFloat

For each vector element, calculates the cosine.

func vsincosf(vFloat, UnsafeMutablePointer&lt;vFloat>) -> vFloat

Simultaneously computes sine and cosine of values in a vector.

func vtanf(vFloat) -> vFloat

For each vector element, calculates the tangent.

func vasinf(vFloat) -> vFloat

For each vector element, calculates the arcsine. Results are in the interval \[-pi/2, pi/2\].

func vacosf(vFloat) -> vFloat

For each vector element, calculates the arccosine. Results are in the interval \[0, pi\].

func vatanf(vFloat) -> vFloat

For each vector element, calculates the arctangent. Results are in the interval \[-pi/2, pi/2\].

func vatan2f(vFloat, vFloat) -> vFloat

For each vector element, calculates the arctangent of `arg2`/`arg1` in the interval \[-pi,pi\] using the sign of both arguments to determine the quadrant of the computed value.

func vvcbrt(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates the cube root for each element of a vector.

