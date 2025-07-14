

- Accelerate
- vDSP
-  subtract(multiplication:multiplication:) 

Type Method

# subtract(multiplication:multiplication:)

Returns the double-precision element-wise difference of the products of two pairs of vectors.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func subtract(
    multiplication multiplicationAB: (a: T, b: U),
    multiplication multiplicationCD: (c: R, d: S)
) -> [Double] where R : AccelerateBuffer, S : AccelerateBuffer, T : AccelerateBuffer, U : AccelerateBuffer, R.Element == Double, S.Element == Double, T.Element == Double, U.Element == Double
```

## Parameters 

`multiplicationAB`  

A tuple that contains the vectors `A` and `B` in `E = (A * B) - (C * D)`.

`multiplicationCD`  

A tuple that contains the vectors `C` and `D` in `E = (A * B) - (C * D)`.

## Return Value

The output vector `E` in `E = (A * B) - (C * D)`.

## Discussion

This function calculates the differences of the first `N` elements of the product of vectors `A` and `B` and the product of vectors `C` and `D`.

```
 for (n = 0; n 

The following code shows an example of using this function:

```
    let a: [Double] = [ 1,  2,  3,  4,  5]
    let b: [Double] = [10, 20, 30, 40, 50]
    let c: [Double] = [ 5,  4,  3,  2,  1]
    let d: [Double] = [50, 40, 30, 20, 10]

    let e = vDSP.subtract(multiplication: (a, b),
                          multiplication: (c, d))

    // Prints "[-240.0, -120.0, 0.0, 120.0, 240.0]".
    print(e)

```

## See Also

### Subtraction

static func subtract&lt;T, U>(U, T) -> [Double]

Returns the double-precision element-wise subtraction of two vectors.

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

static func subtract&lt;R, S, T, U>(multiplication: (a: T, b: U), multiplication: (c: R, d: S)) -> [Float]

Returns the single-precision element-wise difference of the products of two pairs of vectors.

