

- Accelerate
-  vscalbf(\_:\_:) 

Function

# vscalbf(\_:\_:)

For each vector element, calculates x \* 2^n efficiently. This is not normally done by computing 2^n explicitly.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func vscalbf(
    _: vFloat,
    _: vSInt32
) -> vFloat
```

## See Also

### Exponential and Logarithmic Functions (from vfp.h)

func vexpf(vFloat) -> vFloat

For each vector element, calculates the exponential of X.

func vexp2f(vFloat) -> vFloat

func vexpm1f(vFloat) -> vFloat

For each vector element, calculates ExpM1(x) = Exp(x) - 1. But, for small enough arguments, ExpM1(x) is expected to be more accurate than Exp(x) - 1.

func vlogf(vFloat) -> vFloat

For each vector element, calculates the natural logarithm of `X`.

func vlog1pf(vFloat) -> vFloat

For each vector element, calculates Log1P = Log(1 + x). But, for small enough arguments, Log1P is expected to be more accurate than Log(1 + x).

func vlog10f(vFloat) -> vFloat

Computes the base-10 logarithm of values in a vector.

func vlogbf(vFloat) -> vFloat

For each vector element, extracts the exponent of `X`, as a signed integral value. A subnormal argument is treated as though it were first normalized. Thus: 1 \

func vlog2f(vFloat) -> vFloat

func vvpows(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates the cube root for each element of a vector.

func vvpowsf(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates, elementwise, x\*\*y for a vector x and a scalar y.

