

- Accelerate
- vDSP
-  subtract(\_:\_:) 

Type Method

# subtract(\_:\_:)

Returns the double-precision element-wise subtraction of two vectors.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func subtract(
    _ vectorA: U,
    _ vectorB: T
) -> [Double] where T : AccelerateBuffer, U : AccelerateBuffer, T.Element == Double, U.Element == Double
```

## Parameters 

`vectorA`  

The first input vector, `A`.

`vectorB`  

The second input vector, `B`.

## Return Value

The output vector, `C`.

## Discussion

This function calculates the differences of the first `N` elements of input vectors `A` and `B`, and writes the result to output vector `C`.

```
 for (n = 0; n 

The following code shows an example of using this function:

```
    let a: [Double] = [10, 20, 30, 40, 50]
    let b: [Double] = [ 1,  2,  3,  4,  5]

    let c = vDSP.subtract(a, b)

    // Prints "[9.0, 18.0, 27.0, 36.0, 45.0]".
    print(c)
```

## See Also

### Subtraction

static func subtract&lt;T, U>(U, T) -> [Float]

Returns the single-precision element-wise subtraction of two vectors.

static func subtract&lt;T, U, V>(U, T, result: inout V)

Calculates the double-precision element-wise subtraction of two vectors.

static func subtract&lt;T, U, V>(U, T, result: inout V)

Calculates the single-precision element-wise subtraction of two vectors.

static func subtract(DSPSplitComplex, from: DSPSplitComplex, count: Int, result: inout DSPSplitComplex)

Calculates the single-precision elementwise subtraction of a complex vector from a complex vector.

static func subtract(DSPDoubleSplitComplex, from: DSPDoubleSplitComplex, count: Int, result: inout DSPDoubleSplitComplex)

Calculates the double-precision elementwise subtraction of a complex vector from a complex vector.

static func subtract&lt;T, U>(multiplication: (a: U, b: Double), T) -> [Double]

Calculates the double-precision element-wise difference of the product of a vector and a scalar value, and a vector.

static func subtract&lt;S, T, U>(multiplication: (a: T, b: U), S) -> [Double]

Returns the double-precision element-wise difference of a vector and the product of two vectors.

static func subtract&lt;T, U>(multiplication: (a: U, b: Float), T) -> [Float]

Calculates the single-precision element-wise difference of the product of a vector and a scalar value, and a vector.

static func subtract&lt;S, T, U>(multiplication: (a: T, b: U), S) -> [Float]

Returns the single-precision element-wise difference of a vector and the product of two vectors.

static func subtract&lt;T, U, V>(multiplication: (a: U, b: Double), T, result: inout V)

Calculates the double-precision element-wise difference of the product of a vector and a scalar value, and a vector.

static func subtract&lt;T, U, V>(multiplication: (a: U, b: Float), T, result: inout V)

Calculates the single-precision element-wise difference of the product of a vector and a scalar value, and a vector.

static func subtract&lt;S, T, U, V>(multiplication: (a: T, b: U), S, result: inout V)

Calculates the double-precision element-wise difference of a vector and the product of two vectors.

static func subtract&lt;S, T, U, V>(multiplication: (a: T, b: U), S, result: inout V)

Calculates the single-precision element-wise difference of a vector and the product of two vectors.

static func subtract&lt;R, S, T, U>(multiplication: (a: T, b: U), multiplication: (c: R, d: S)) -> [Double]

Returns the double-precision element-wise difference of the products of two pairs of vectors.

static func subtract&lt;R, S, T, U>(multiplication: (a: T, b: U), multiplication: (c: R, d: S)) -> [Float]

Returns the single-precision element-wise difference of the products of two pairs of vectors.

