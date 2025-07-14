

- Accelerate
-  vsinf(\_:) 

Function

# vsinf(\_:)

For each vector element, calculates the sine.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func vsinf(_: vFloat) -> vFloat
```

## See Also

### Trigonometric Functions (from vfp.h)

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

func vvcbrtf(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates the cube root for each element of a vector.

