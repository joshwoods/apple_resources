

- Accelerate
-  vvexp2f(\_:\_:\_:) 

Function

# vvexp2f(\_:\_:\_:)

Calculates 2 raised to the power of each element in an array of single-precision values.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func vvexp2f(
    _: UnsafeMutablePointer,
    _: UnsafePointer,
    _: UnsafePointer
)
```

### Parameters:

parameter 1  
The output array, *y*.

parameter 2  
The input array, *x*.

parameter 3  
The number of elements in the arrays.

## See Also

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

