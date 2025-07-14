

- Accelerate
-  vForce 

API Collection

# vForce

Perform transcendental and trigonometric functions on vectors of any length.

## Overview

The vForce library provides a range of trigonometric and transcendental functions that work over large collections of single- and double-precision values. The collections can be of any length, and vForce supplies vectorized functions for the current architecture.

The functions declared in the vForce library have the customary mathematical names, but with the prefix `vv`, for example, vvsqrtf(_:_:_:). Each mathematical function is available in two variants: one for single-precision data and one for double-precision data. The single-precision forms have the suffix `f`, whereas the double-precision forms have no suffix. For example, vvcosf(_:_:_:) is the single-precision cosine function, and vvcos(_:_:_:) is the double-precision variant.

All of the vForce library functions follow a common format:

- The return type is `void`.

- The first parameter points to an array to hold the results. The only exceptions are vvsincosf(_:_:_:_:) and vvsincos(_:_:_:_:), which have two result arrays that the first two parameters point to.

- One or more parameters point to operand arrays that are the same length as the result array.

- The last parameter is the array length.

Note

Unless otherwise mentioned, vForce functions work in-place. That is, the input may exactly equal the output.

### Using vForce

The vForce library provides a high-performance alternative to `for` loops and `map(_:)` when applying operations on arrays of floating-point values.

For example, given an arbitrarily sized array, `x`, that contains single-precision values, the following code uses `map(_:)` to create a second array, `y`. On return, `y` contains the square root of each array element.

```
let n = 10_000

let x = (0..

The equivalent functionality implemented in vForce runs significantly faster:

```
let y = [Float](unsafeUninitializedCapacity: n) { buffer, initializedCount in
    vForce.sqrt(x,
                result: &buffer)

    initializedCount = n
}
```

## Topics

### Swift Overlay

enum vForce

An enumeration that acts as a namespace for Swift overlays to vForce.

### Array-Oriented Arithmetic and Auxiliary Functions

static func ceil&lt;U>(U) -> [Double]

Returns the ceiling of each element in a vector of double-precision values.

static func ceil&lt;U>(U) -> [Float]

Returns the ceiling of each element in a vector of single-precision values.

static func ceil&lt;U, V>(U, result: inout V)

Calculates the ceiling of each element in a vector of double-precision values.

static func ceil&lt;U, V>(U, result: inout V)

Calculates the ceiling of each element in a vector of single-precision values.

static func copysign&lt;U, V>(magnitudes: U, signs: V) -> [Double]

Returns each single-precision element in the magnitudes vector, setting its sign to the corresponding elements in the signs vector.

static func copysign&lt;U, V>(magnitudes: U, signs: V) -> [Float]

Returns each single-precision element in the magnitudes vector, setting its sign to the corresponding elements in the signs vector.

static func copysign&lt;T, U, V>(magnitudes: T, signs: U, result: inout V)

Calculates each double-precision element in the magnitudes vector, setting its sign to the corresponding elements in the signs vector.

static func copysign&lt;T, U, V>(magnitudes: T, signs: U, result: inout V)

Calculates each single-precision element in the magnitudes vector, setting its sign to the corresponding elements in the signs vector.

static func floor&lt;U>(U) -> [Double]

Returns the floor of each element in a vector of double-precision values.

static func floor&lt;U>(U) -> [Float]

Returns the floor of each element in a vector of single-precision values.

static func floor&lt;U, V>(U, result: inout V)

Calculates the floor of each element in a vector of double-precision values.

static func floor&lt;U, V>(U, result: inout V)

Calculates the floor of each element in a vector of single-precision values.

static func nearestInteger&lt;U>(U) -> [Double]

Returns the nearest integer to each element in a vector of double-precision values.

static func nearestInteger&lt;U>(U) -> [Float]

Returns the nearest integer to each element in a vector of single-precision values.

static func nearestInteger&lt;U, V>(U, result: inout V)

Calculates the nearest integer to each element in a vector of double-precision values.

static func nearestInteger&lt;U, V>(U, result: inout V)

Calculates the nearest integer to each element in a vector of double-precision values.

static func reciprocal&lt;U>(U) -> [Double]

Returns the reciprocal of each element in a vector of double-precision values.

static func reciprocal&lt;U>(U) -> [Float]

Returns the reciprocal of each element in a vector of single-precision values.

static func reciprocal&lt;U, V>(U, result: inout V)

Calculates the reciprocal of each element in a vector of double-precision values.

static func reciprocal&lt;U, V>(U, result: inout V)

Calculates the reciprocal of each element in a vector of single-precision values.

static func remainder&lt;U, V>(dividends: U, divisors: V) -> [Double]

Returns the remainder of the double-precision elements in `dividends` divided by the elements in `divisors`, using truncating division.

static func remainder&lt;U, V>(dividends: U, divisors: V) -> [Float]

Returns the remainder of the single-precision elements in `dividends` divided by the elements in `divisors`, using truncating division.

static func remainder&lt;T, U, V>(dividends: T, divisors: U, result: inout V)

Calculates the remainder of the double-precision elements in `dividends` divided by the elements in `divisors`, using truncating division.

static func remainder&lt;T, U, V>(dividends: T, divisors: U, result: inout V)

Calculates the remainder of the single-precision elements in `dividends` divided by the elements in `divisors`, using truncating division.

static func rsqrt&lt;U>(U) -> [Double]

Returns the reciprocal square root of each element in a vector of double-precision values.

static func rsqrt&lt;U>(U) -> [Float]

Returns the reciprocal square root of each element in a vector of single-precision values.

static func rsqrt&lt;U, V>(U, result: inout V)

Calculates the reciprocal square root of each element in a vector of double-precision values.

static func rsqrt&lt;U, V>(U, result: inout V)

Calculates the reciprocal square root of each element in a vector of single-precision values.

static func sqrt&lt;U>(U) -> [Double]

Returns the square root of each element in a vector of double-precision values.

static func sqrt&lt;U>(U) -> [Float]

Returns the square root each element in a vector of single-precision values.

static func sqrt&lt;U, V>(U, result: inout V)

Calculates the square root of each element in a vector of double-precision values.

static func sqrt&lt;U, V>(U, result: inout V)

Calculates the square root of each element in a vector of single-precision values.

static func trunc&lt;U>(U) -> [Double]

Returns the integer truncation of each element in a vector of double-precision values.

static func trunc&lt;U>(U) -> [Float]

Returns the integer truncation of each element in a vector of single-precision values.

static func trunc&lt;U, V>(U, result: inout V)

Calculates the integer truncation of each element in a vector of double-precision values.

static func trunc&lt;U, V>(U, result: inout V)

Calculates the integer truncation of each element in a vector of single-precision values.

static func truncatingRemainder&lt;U, V>(dividends: U, divisors: V) -> [Double]

Returns the remainder of the double-precision elements in `dividends` divided by the elements in `divisors`, using truncating division.

static func truncatingRemainder&lt;U, V>(dividends: U, divisors: V) -> [Float]

Returns the remainder of the single-precision elements in `dividends` divided by the elements in `divisors`, using truncating division.

static func truncatingRemainder&lt;T, U, V>(dividends: T, divisors: U, result: inout V)

Calculates the remainder of the double-precision elements in `dividends` divided by the elements in `divisors`, using truncating division.

static func truncatingRemainder&lt;T, U, V>(dividends: T, divisors: U, result: inout V)

Calculates the remainder of the single-precision elements in `dividends` divided by the elements in `divisors`, using truncating division.

func vvceil(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates the ceiling of each element in an array of double-precision values.

func vvceilf(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates the ceiling of each element in an array of single-precision values.

func vvfloor(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates the floor of each element in an array of double-precision values.

func vvfloorf(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates the floor of each element in an array of single-precision values.

func vvcopysign(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Copies an array, setting the sign of each element based on a second array of double-precision values.

func vvcopysignf(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Copies an array, setting the sign of each element based on a second array of single-precision values.

func vvdiv(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Divides each element in an array by the corresponding value in a second array of double-precision values.

func vvdivf(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Divides each element in an array by the corresponding value in a second array of single-precision values.

func vvfabs(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates the absolute value for each element in an array of double-precision values.

func vvfabsf(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates the absolute value for each element in an array of single-precision values.

func vvfmod(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates the modulus after dividing each element in an array by the corresponding element in a second array of double-precision values.

func vvfmodf(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates the modulus after dividing each element in an array by the corresponding element in a second array of single-precision values.

func vvremainder(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates the remainder after dividing each element in an array by the corresponding element in a second array of double-precision values.

func vvremainderf(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates the remainder after dividing each element in an array by the corresponding element in a second array of single-precision values.

func vvint(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates the integer truncation for each element in an array of double-precision values.

func vvintf(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates the integer truncation for each element in an array of single-precision values.

func vvnint(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates the nearest integer for each element in an array of double-precision values.

func vvnintf(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates the nearest integer for each element in an array of single-precision values.

func vvrsqrt(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates the reciprocal square root of each element in an array of double-precision values.

func vvrsqrtf(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates the reciprocal square root of each element in an array of single-precision values.

func vvsqrt(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates the square root of each element in an array of double-precision values.

func vvsqrtf(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates the square root of each element in an array of single-precision values.

func vvrec(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates the reciprocal of each element in an array of double-precision values.

func vvrecf(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates the reciprocal of each element in an array of single-precision values.

func vvnextafter(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates the next machine-representable value for each element in an array of double-precision values.

func vvnextafterf(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates the next machine-representable value for each element in an array of single-precision values.

### Array-Oriented Exponential and Logarithmic Functions

static func exp&lt;U>(U) -> [Double]

Returns the *e*, raised to the power of each element in a vector of double-precision values.

static func exp&lt;U>(U) -> [Float]

Returns the *e*, raised to the power of each element in a vector of single-precision values.

static func exp&lt;U, V>(U, result: inout V)

Calculates the *e*, raised to the power of each element in a vector of double-precision values.

static func exp&lt;U, V>(U, result: inout V)

Calculates the *e*, raised to the power of each element in a vector of single-precision values.

static func exp2&lt;U>(U) -> [Double]

Returns the 2, raised to the power of each element in a vector of double-precision values.

static func exp2&lt;U>(U) -> [Float]

Returns the 2, raised to the power of each element in a vector of single-precision values.

static func exp2&lt;U, V>(U, result: inout V)

Calculates the 2, raised to the power of each element in a vector of double-precision values.

static func exp2&lt;U, V>(U, result: inout V)

Calculates the 2, raised to the power of each element in a vector of single-precision values.

static func expm1&lt;U>(U) -> [Double]

Returns the *eˣ-1* for each element in a vector of double-precision values.

static func expm1&lt;U>(U) -> [Float]

Returns the *eˣ-1* for each element in a vector of single-precision values.

static func expm1&lt;U, V>(U, result: inout V)

Calculates the *eˣ-1* for each element in a vector of double-precision values.

static func expm1&lt;U, V>(U, result: inout V)

Calculates the *eˣ-1* for each element in a vector of single-precision values.

static func log10&lt;U>(U) -> [Double]

Returns the base 10 logarithm of each element in a vector of double-precision values.

static func log&lt;U>(U) -> [Double]

Returns the natural logarithm for each element in a vector of double-precision values.

static func log&lt;U>(U) -> [Float]

Returns the natural logarithm for each element in a vector of single-precision values.

static func log&lt;U, V>(U, result: inout V)

Calculates the natural logarithm for each element in a vector of double-precision values.

static func log&lt;U, V>(U, result: inout V)

Calculates the natural logarithm for each element in a vector of single-precision values.

static func log1p&lt;U>(U) -> [Double]

Returns *log(1+x)* for each element in a vector of double-precision values.

static func log1p&lt;U>(U) -> [Float]

Returns *log(1+x)* for each element in a vector of single-precision values.

static func log1p&lt;U, V>(U, result: inout V)

Calculates *log(1+x)* for each element in a vector of double-precision values.

static func log1p&lt;U, V>(U, result: inout V)

Calculates *log(1+x)* for each element in a vector of single-precision values.

static func log10&lt;U>(U) -> [Float]

Returns the base 10 logarithm of each element in a vector of single-precision values.

static func log10&lt;U, V>(U, result: inout V)

Calculates the base 10 logarithm of each element in a vector of double-precision values.

static func log10&lt;U, V>(U, result: inout V)

Calculates the base 10 logarithm of each element in a vector of single-precision values.

static func log2&lt;U>(U) -> [Double]

Returns the base 2 logarithm of each element in a vector of double-precision values.

static func log2&lt;U>(U) -> [Float]

Returns the base 2 logarithm of each element in a vector of single-precision values.

static func log2&lt;U, V>(U, result: inout V)

Calculates the base 2 logarithm of each element in a vector of double-precision values.

static func log2&lt;U, V>(U, result: inout V)

Calculates the base 2 logarithm of each element in a vector of single-precision values.

static func logb&lt;U>(U) -> [Double]

Returns the unbiased exponent of each element in a vector of double-precision values.

static func logb&lt;U>(U) -> [Float]

Returns the unbiased exponent of each element in a vector of double-precision values.

static func logb&lt;U, V>(U, result: inout V)

Calculates the unbiased exponent of each element in a vector of double-precision values.

static func logb&lt;U, V>(U, result: inout V)

Calculates the unbiased exponent of each element in a vector of single-precision values.

func vvexp(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates *e* raised to the power of each element in an array of double-precision values.

func vvexpf(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates *e* raised to the power of each element in an array of single-precision values.

func vvexp2(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates 2 raised to the power of each element in an array of double-precision values.

func vvexp2f(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates 2 raised to the power of each element in an array of single-precision values.

func vvexpm1(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates *eˣ-1* for each element in an array of double-precision values.

func vvexpm1f(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates *eˣ-1* for each element in an array of single-precision values.

func vvlog(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates the natural logarithm for each element in an array of double-precision values.

func vvlogf(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates the natural logarithm for each element in an array of single-precision values.

func vvlog1p(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates *log(1+x)* for each element in an array of double-precision values.

func vvlog1pf(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates *log(1+x)* for each element in an array of single-precision values.

func vvlog2(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates the base 2 logarithm of each element in an array of double-precision values.

func vvlog2f(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates the base 2 logarithm of each element in an array of single-precision values.

func vvlog10(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates the base 10 logarithm of each element in an array of double-precision values.

func vvlog10f(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates the base 10 logarithm of each element in an array of single-precision values.

func vvlogb(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates the unbiased exponent of each element in an array of double-precision values.

func vvlogbf(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates the unbiased exponent of each element in an array of single-precision values.

### Array-Oriented Power Functions

static func pow&lt;U, V>(bases: U, exponents: V) -> [Double]

Returns each double-precision element in the bases vector, raised to the power of the corresponding element in the exponents vector.

static func pow&lt;U, V>(bases: U, exponents: V) -> [Float]

Returns each single-precision element in the bases vector, raised to the power of the corresponding element in the exponents vector.

static func pow&lt;T, U, V>(bases: T, exponents: U, result: inout V)

Calculates each double-precision element in the bases vector, raised to the power of the corresponding element in the exponents vector.

static func pow&lt;T, U, V>(bases: T, exponents: U, result: inout V)

Calculates each single-precision element in the bases vector, raised to the power of the corresponding element in the exponents vector.

func vvpow(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Raises each element in an array to the power of the corresponding element in a second array of double-precision values.

func vvpowf(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Raises each element in an array to the power of the corresponding element in a second array of single-precision values.

### Array-Oriented Trigonometric Functions

static func acos&lt;U>(U) -> [Double]

Returns the arccosine of each element in a vector of double-precision values.

static func acos&lt;U>(U) -> [Float]

Returns the arccosine of each element in a vector of single-precision values.

static func acos&lt;U, V>(U, result: inout V)

Calculates the arccosine of each element in a vector of double-precision values.

static func acos&lt;U, V>(U, result: inout V)

Calculates the arccosine of each element in a vector of single-precision values.

static func asin&lt;U>(U) -> [Double]

Returns the arcsine of each element in a vector of double-precision values.

static func asin&lt;U>(U) -> [Float]

Returns the arcsine of each element in a vector of single-precision values.

static func asin&lt;U, V>(U, result: inout V)

Calculates the arcsine of each element in a vector of double-precision values.

static func asin&lt;U, V>(U, result: inout V)

Calculates the arcsine of each element in a vector of single-precision values.

static func atan&lt;U>(U) -> [Double]

Returns the arctangent of each element in a vector of double-precision values.

static func atan&lt;U>(U) -> [Float]

Returns the arctangent of each element in a vector of single-precision values.

static func atan&lt;U, V>(U, result: inout V)

Calculates the arctangent of each element in a vector of double-precision values.

static func atan&lt;U, V>(U, result: inout V)

Calculates the arctangent of each element in a vector of single-precision values.

static func atan2&lt;U, V>(x: U, y: V) -> [Double]

Returns the arctangent of each pair of elements in two vectors of double-precision values.

static func atan2&lt;U, V>(x: U, y: V) -> [Float]

Returns the arctangent of each pair of elements in two vectors of single-precision values.

static func atan2&lt;T, U, V>(x: T, y: U, result: inout V)

Calculates the arctangent of each pair of elements in two vectors of double-precision values.

static func atan2&lt;T, U, V>(x: T, y: U, result: inout V)

Calculates the arctangent of each pair of elements in two vectors of single-precision values.

static func cos&lt;U>(U) -> [Double]

Returns the cosine of each element in a vector of double-precision values.

static func cos&lt;U>(U) -> [Float]

Returns the cosine of each element in a vector of single-precision values.

static func cos&lt;U, V>(U, result: inout V)

Calculates the cosine of each element in a vector of double-precision values.

static func cos&lt;U, V>(U, result: inout V)

Calculates the cosine of each element in a vector of single-precision values.

static func cosPi&lt;U>(U) -> [Double]

Returns the cosine of pi, multiplied by each element in a vector of double-precision values.

static func cosPi&lt;U>(U) -> [Float]

Returns the cosine of pi, multiplied by each element in a vector of single-precision values.

static func cosPi&lt;U, V>(U, result: inout V)

Calculates the cosine of pi, multiplied by each element in a vector of double-precision values.

static func cosPi&lt;U, V>(U, result: inout V)

Calculates the cosine of pi, multiplied by each element in a vector of single-precision values.

static func sin&lt;U>(U) -> [Double]

Returns the sine of each element in a vector of double-precision values.

static func sin&lt;U>(U) -> [Float]

Returns the sine of each element in a vector of single-precision values.

static func sin&lt;U, V>(U, result: inout V)

Calculates the sine of each element in a vector of double-precision values.

static func sin&lt;U, V>(U, result: inout V)

Calculates the sine of each element in a vector of single-precision values.

static func sinPi&lt;U>(U) -> [Double]

Returns the sine of pi, multiplied by each element in a vector of double-precision values.

static func sinPi&lt;U>(U) -> [Float]

Returns the sine of pi, multiplied by each element in a vector of single-precision values.

static func sinPi&lt;U, V>(U, result: inout V)

Calculates the sine of pi, multiplied by each element in a vector of double-precision values.

static func sinPi&lt;U, V>(U, result: inout V)

Calculates the sine of pi, multiplied by each element in a vector of single-precision values.

static func sincos&lt;T, U, V>(T, sinResult: inout U, cosResult: inout V)

Calculates the sine and cosine of each element in a vector of double-precision values.

static func sincos&lt;T, U, V>(T, sinResult: inout U, cosResult: inout V)

Calculates the sine and cosine of each element in a vector of double-precision values.

static func tan&lt;U>(U) -> [Double]

Returns the tangent of each element in a vector of double-precision values.

static func tan&lt;U>(U) -> [Float]

Returns the tangent of each element in a vector of single-precision values.

static func tan&lt;U, V>(U, result: inout V)

Calculates the tangent of each element in a vector of double-precision values.

static func tan&lt;U, V>(U, result: inout V)

Calculates the tangent of each element in a vector of single-precision values.

static func tanPi&lt;U>(U) -> [Double]

Returns the tangent of pi, multiplied by each element in a vector of double-precision values.

static func tanPi&lt;U>(U) -> [Float]

Returns the tangent of pi, multiplied by each element in a vector of single-precision values.

static func tanPi&lt;U, V>(U, result: inout V)

Calculates the tangent of pi, multiplied by each element in a vector of double-precision values.

static func tanPi&lt;U, V>(U, result: inout V)

Calculates the tangent of pi, multiplied by each element in a vector of single-precision values.

func vvsin(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates the sine of each element in an array of double-precision values.

func vvsinf(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates the sine of each element in an array of single-precision values.

func vvsinpi(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates the sine of pi multiplied by each element in an array of double-precision values.

func vvsinpif(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates the sine of pi multiplied by each element in an array of single-precision values.

func vvcos(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates the cosine of each element in an array of double-precision values.

func vvcosf(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates the cosine of each element in an array of single-precision values.

func vvcospi(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates the cosine of pi multiplied by each element in an array of double-precision values.

func vvcospif(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates the cosine of pi multiplied by each element in an array of single-precision values.

func vvcosisin(OpaquePointer, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates the cosine and sine of each element in an array of double-precision values.

func vvcosisinf(OpaquePointer, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates the cosine and sine of each element in an array of single-precision values.

func vvsincos(UnsafeMutablePointer&lt;Double>, UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates the cosine and sine of each element in an array of double-precision values.

func vvsincosf(UnsafeMutablePointer&lt;Float>, UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates the cosine and sine of each element in an array of single-precision values.

func vvtan(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates the tangent of each element in an array of double-precision values.

func vvtanf(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates the tangent of each element in an array of single-precision values.

func vvtanpi(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates the tangent of pi multiplied by each element in an array of double-precision values.

func vvtanpif(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates the tangent of pi multiplied by each element in an array of single-precision values.

func vvasin(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates the arcsine of each element in an array of double-precision values.

func vvasinf(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates the arcsine of each element in an array of single-precision values.

func vvacos(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates the arccosine of each element in an array of double-precision values.

func vvacosf(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates the arccosine of each element in an array of single-precision values.

func vvatan(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates the arctangent of each element in an array of double-precision values.

func vvatanf(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates the arctangent of each element in an array of single-precision values.

func vvatan2(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates the arctangent of each pair of elements in two arrays of double-precision values.

func vvatan2f(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates the arctangent of each pair of elements in two arrays of single-precision values.

### Array-Oriented Hyperbolic Functions

static func acosh&lt;U>(U) -> [Double]

Returns the inverse hyperbolic cosine of each element in a vector of double-precision values.

static func acosh&lt;U>(U) -> [Float]

Returns the inverse hyperbolic cosine of each element in a vector of single-precision values.

static func acosh&lt;U, V>(U, result: inout V)

Calculates the inverse hyperbolic cosine of each element in a vector of double-precision values.

static func acosh&lt;U, V>(U, result: inout V)

Calculates the inverse hyperbolic cosine of each element in a vector of single-precision values.

static func asinh&lt;U>(U) -> [Double]

Returns the inverse hyperbolic sine of each element in a vector of double-precision values.

static func asinh&lt;U>(U) -> [Float]

Returns the inverse hyperbolic sine of each element in a vector of single-precision values.

static func asinh&lt;U, V>(U, result: inout V)

Calculates the inverse hyperbolic sine of each element in a vector of double-precision values.

static func asinh&lt;U, V>(U, result: inout V)

Calculates the inverse hyperbolic sine of each element in a vector of single-precision values.

static func atanh&lt;U>(U) -> [Double]

Returns the inverse hyperbolic tangent of each element in a vector of double-precision values.

static func atanh&lt;U>(U) -> [Float]

Returns the inverse hyperbolic tangent of each element in a vector of single-precision values.

static func atanh&lt;U, V>(U, result: inout V)

Calculates the inverse hyperbolic tangent of each element in a vector of double-precision values.

static func atanh&lt;U, V>(U, result: inout V)

Calculates the inverse hyperbolic tangent of each element in a vector of single-precision values.

static func cosh&lt;U>(U) -> [Double]

Returns the hyperbolic cosine of each element in a vector of double-precision values.

static func cosh&lt;U>(U) -> [Float]

Returns the hyperbolic cosine of each element in a vector of single-precision values.

static func cosh&lt;U, V>(U, result: inout V)

Calculates the hyperbolic cosine of each element in a vector of double-precision values.

static func cosh&lt;U, V>(U, result: inout V)

Calculates the hyperbolic cosine of each element in a vector of single-precision values.

static func sinh&lt;U>(U) -> [Double]

Returns the hyperbolic sine of each element in a vector of double-precision values.

static func sinh&lt;U>(U) -> [Float]

Returns the hyperbolic sine of each element in a vector of single-precision values.

static func sinh&lt;U, V>(U, result: inout V)

Calculates the hyperbolic sine of each element in a vector of double-precision values.

static func sinh&lt;U, V>(U, result: inout V)

Calculates the hyperbolic sine of each element in a vector of single-precision values.

static func tanh&lt;U>(U) -> [Double]

Returns the hyperbolic tangent of each element in a vector of double-precision values.

static func tanh&lt;U>(U) -> [Float]

Returns the hyperbolic tangent of each element in a vector of single-precision values.

static func tanh&lt;U, V>(U, result: inout V)

Calculates the hyperbolic tangent of each element in a vector of double-precision values.

static func tanh&lt;U, V>(U, result: inout V)

Calculates the hyperbolic tangent of each element in a vector of single-precision values.

func vvsinh(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates the hyperbolic sine of each element in an array of double-precision values.

func vvsinhf(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates the hyperbolic sine of each element in an array of single-precision values.

func vvcosh(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates the hyperbolic cosine of each element in an array of double-precision values.

func vvcoshf(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates the hyperbolic cosine of each element in an array of single-precision values.

func vvtanh(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates the hyperbolic tangent of each element in an array of double-precision values.

func vvtanhf(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates the hyperbolic tangent of each element in an array of single-precision values.

func vvasinh(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates the inverse hyperbolic sine of each element in an array of double-precision values.

func vvasinhf(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates the inverse hyperbolic sine of each element in an array of single-precision values.

func vvacosh(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates the inverse hyperbolic cosine of each element in an array of double-precision values.

func vvacoshf(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates the inverse hyperbolic cosine of each element in an array of single-precision values.

func vvatanh(UnsafeMutablePointer&lt;Double>, UnsafePointer&lt;Double>, UnsafePointer&lt;Int32>)

Calculates the inverse hyperbolic tangent of each element in an array of double-precision values.

func vvatanhf(UnsafeMutablePointer&lt;Float>, UnsafePointer&lt;Float>, UnsafePointer&lt;Int32>)

Calculates the inverse hyperbolic tangent of each element in an array of single-precision values.

### Data Types

typealias COMPLEX

typealias DOUBLE_COMPLEX

## See Also

### Vectors, Matrices, and Quaternions

Working with Vectors

Use vectors to calculate geometric values, calculate dot products and cross products, and interpolate between values.

Working with Matrices

Solve simultaneous equations and transform points in space.

Working with Quaternions

Rotate points around the surface of a sphere, and interpolate between them.

Rotating a cube by transforming its vertices

Rotate a cube through a series of keyframes using quaternion interpolation to transition between them.

simd

Perform computations on small vectors and matrices.

