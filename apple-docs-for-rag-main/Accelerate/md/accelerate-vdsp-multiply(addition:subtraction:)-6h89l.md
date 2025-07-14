

- Accelerate
- vDSP
-  multiply(addition:subtraction:) 

Type Method

# multiply(addition:subtraction:)

Returns the single-precision element-wise product of the sum of two vectors and the difference of two vectors.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func multiply(
    addition: (a: R, b: S),
    subtraction: (c: T, d: U)
) -> [Float] where R : AccelerateBuffer, S : AccelerateBuffer, T : AccelerateBuffer, U : AccelerateBuffer, R.Element == Float, S.Element == Float, T.Element == Float, U.Element == Float
```

## Parameters 

`addition`  

A tuple that contains the vectors `A` and `B` in `E = (A + B) * (C - D)`.

`subtraction`  

A tuple that contains the vectors `C` and `D` in `E = (A + B) * (C - D)`.

## Return Value

The output vector `E` in `E = (A + B) * (C - D)`.

## Mentioned in 

Using vDSP for vector-based arithmetic

## Discussion

This function calculates the products of the first `N` elements of the addition of vectors `A` and `B` and the subtraction of vectors `C` and `D`.

```
 for (n = 0; n 

The following code shows an example of using this function:

```
    let a: [Float] = [ 1,  2,  3,  4,  5]
    let b: [Float] = [10, 20, 30, 40, 50]
    let c: [Float] = [ 5,  4,  3,  2,  1]
    let d: [Float] = [50, 40, 30, 20, 10]

    let e = vDSP.multiply(addition: (a, b),
                          subtraction: (c, d))

    // Prints "[-495.0, -792.0, -891.0, -792.0, -495.0]".
    print(e)

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

static func multiply&lt;T, U>(addition: (a: T, b: U), Double) -> [Double]

Returns the double-precision element-wise product of the sum of two vectors and a scalar value.

static func multiply&lt;S, T, U>(addition: (a: S, b: T), U) -> [Double]

Returns the double-precision element-wise product of a vector and the sum of two vectors.

static func multiply&lt;T, U>(addition: (a: T, b: U), Float) -> [Float]

Returns the single-precision element-wise product of the sum of two vectors and a scalar value.

