

- Accelerate
- vDSP
-  multiply(\_:\_:) 

Type Method

# multiply(\_:\_:)

Returns the double-precision element-wise product of two vectors.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func multiply(
    _ vectorA: T,
    _ vectorB: U
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

This function calculates the products of the first `N` elements of input vectors `A` and `B`, and writes the result to output vector `C`.

```
 for (n = 0; n 

The following code shows an example of using this function:

```
    let a: [Double] = [10, 20, 30, 40, 50]
    let b: [Double] = [ 1,  2,  3,  4,  5]

    let c = vDSP.multiply(a, b)

    // Prints "[10.0, 40.0, 90.0, 160.0, 250.0]".
    print(c)
```

## See Also

### Multiplication

static func multiply&lt;U>(Double, U) -> [Double]

Returns the double-precision element-wise product of a vector and a scalar value.

static func multiply&lt;U>(Float, U) -> [Float]

Returns the single-precision element-wise product of a vector and a scalar value.

static func multiply&lt;T, U>(T, U) -> [Float]

Returns the single-precision element-wise product of two vectors.

static func multiply&lt;U, V>(Double, U, result: inout V)

Calculates the double-precision element-wise product of a vector and a scalar value.

static func multiply&lt;U, V>(Float, U, result: inout V)

Calculates the single-precision element-wise product of a vector and a scalar value.

static func multiply&lt;T, U, V>(T, U, result: inout V)

Calculates the double-precision element-wise product of two vectors.

static func multiply&lt;T, U, V>(T, U, result: inout V)

Calculates the single-precision element-wise product of two vectors.

static func multiply(DSPSplitComplex, by: DSPSplitComplex, count: Int, useConjugate: Bool, result: inout DSPSplitComplex)

Calculates the product of two complex single-precision vectors, optionally conjugating one of them.

static func multiply(DSPDoubleSplitComplex, by: DSPDoubleSplitComplex, count: Int, useConjugate: Bool, result: inout DSPDoubleSplitComplex)

Calculates the elementwise product of two complex double-precision vectors, optionally conjugating one of them.

static func multiply&lt;U>(DSPSplitComplex, by: U, result: inout DSPSplitComplex)

Calculates the double-precision elementwise product of a complex vector and a real vector.

static func multiply&lt;U>(DSPDoubleSplitComplex, by: U, result: inout DSPDoubleSplitComplex)

Calculates the single-precision elementwise product of a complex vector and a real vector.

static func multiply&lt;T, U>(addition: (a: T, b: U), Double) -> [Double]

Returns the double-precision element-wise product of the sum of two vectors and a scalar value.

static func multiply&lt;S, T, U>(addition: (a: S, b: T), U) -> [Double]

Returns the double-precision element-wise product of a vector and the sum of two vectors.

static func multiply&lt;T, U>(addition: (a: T, b: U), Float) -> [Float]

Returns the single-precision element-wise product of the sum of two vectors and a scalar value.

static func multiply&lt;S, T, U>(addition: (a: S, b: T), U) -> [Float]

Returns the single-precision element-wise product of a vector and the sum of two vectors.

