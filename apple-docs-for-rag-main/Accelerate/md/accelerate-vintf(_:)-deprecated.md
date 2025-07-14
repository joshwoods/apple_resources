

- Accelerate
-  vintf(\_:) Deprecated

Function

# vintf(\_:)

Truncates the decimal portion of a vector of floating-point values.

macOS 10.5–10.14Deprecated

``` source
func vintf(_: vFloat) -> vFloat
```

## Return Value

Returns a vector of floating-point values, each of which is the result of truncating the fractional portion of the corresponding value in `A`.

### Parameters

A  
The source vector

## See Also

### Floating-Point Arithmetic and Auxiliary Functions (from vfp.h)

func vceilf(vFloat) -> vFloat

Computes the ceiling of values in a vector of floating-point values.

func vcopysignf(vFloat, vFloat) -> vFloat

For each vector element, produces a value with the magnitude of `arg2` and sign `arg1`. Note that the order of the arguments matches the recommendation of the IEEE 754 floating-point standard, which is opposite from the SANE copysign function.

func vdivf(vFloat, vFloat) -> vFloat

For each vector element, calculates `A`/`B`.

func vfabf(vFloat) -> vFloat

For each vector element, calculates the absolute value of `v`.

Deprecated

func vfabsf(vFloat) -> vFloat

func vfloorf(vFloat) -> vFloat

Computes the floor of values in a vector of floating-point values.

func vnintf(vFloat) -> vFloat

Rounds to the nearest integer (nearest even for ties).

func vnextafterf(vFloat, vFloat) -> vFloat

For each vector element, calculates the next representable value after `x` in the direction of `y`. If `x` is equal to `y`, then `y` is returned.

func vrecf(vFloat) -> vFloat

Computes the reciprocal of values in a vector.

func vrsqrtf(vFloat) -> vFloat

For each vector element, calculates the inverse of the square root of `X`.

func vsqrtf(vFloat) -> vFloat

For each vector element, calculates the square root of `X`.

func vtablelookup(vSInt32, UnsafeMutablePointer&lt;UInt32>) -> vUInt32

For each vector element of `Index_Vect`, returns the corresponding value from `Table`.

func vtruncf(vFloat) -> vFloat

