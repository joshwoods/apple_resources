

- Accelerate
- vDSP
-  multiply(addition:\_:) 

Type Method

# multiply(addition:\_:)

Returns the double-precision element-wise product of the sum of two vectors and a scalar value.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func multiply(
    addition: (a: T, b: U),
    _ scalar: Double
) -> [Double] where T : AccelerateBuffer, U : AccelerateBuffer, T.Element == Double, U.Element == Double
```

## Parameters 

`addition`  

A tuple that contains the vectors `A` and `B` in `D = (A + B) * C`.

`scalar`  

The input scalar value `C` in `D = (A + B) * C`.

## Return Value

The output vector `D` in `D = (A + B) * C`.

## Discussion

This function calculates the element-wise sum of vectors `A` and `B`, multiplies the sum by scalar value `C`, and writes the result to vector `D`.

```
 for (n = 0; n 

The following code shows an example of using this function:

```
    let a: [Double] = [ 1,  2,  3,  4,  5]
    let b: [Double] = [10, 20, 30, 40, 50]
    let c: Double = 5

    let d = vDSP.multiply(addition: (a, b),
                          c)

    // Prints "[55.0, 110.0, 165.0, 220.0, 275.0]".
    print(d)
```

## See Also

### Multiplication

static func multiply&lt;U>(Double, U) -> [Double]

Returns the double-precision element-wise product of a vector and a scalar value.

static func multiply&lt;T, U>(T, U) -> [Double]

Returns the double-precision element-wise product of two vectors.

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

static func multiply&lt;S, T, U>(addition: (a: S, b: T), U) -> [Double]

Returns the double-precision element-wise product of a vector and the sum of two vectors.

static func multiply&lt;T, U>(addition: (a: T, b: U), Float) -> [Float]

Returns the single-precision element-wise product of the sum of two vectors and a scalar value.

static func multiply&lt;S, T, U>(addition: (a: S, b: T), U) -> [Float]

Returns the single-precision element-wise product of a vector and the sum of two vectors.

