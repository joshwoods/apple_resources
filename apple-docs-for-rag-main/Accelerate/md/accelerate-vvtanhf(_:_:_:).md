

- Accelerate
-  vvtanhf(\_:\_:\_:) 

Function

# vvtanhf(\_:\_:\_:)

Calculates the hyperbolic tangent of each element in an array of single-precision values.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func vvtanhf(
    _: UnsafeMutablePointer,
    _: UnsafePointer,
    _: UnsafePointer
)
```

## Discussion

### Parameters

parameter 1  
The output array, *y*.

parameter 2  
The input array, *x*.

parameter 3  
The number of elements in the arrays.

If `x` is `+/-0`, the result preserves the signed zero.

If `x` is `+/-inf`, the result is `+/-1`.

## See Also

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

