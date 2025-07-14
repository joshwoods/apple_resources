

- Accelerate
- vDSP
-  divide(\_:\_:result:) 

Type Method

# divide(\_:\_:result:)

Calculates the single-precision element-wise division of two vectors.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func divide(
    _ vectorA: T,
    _ vectorB: U,
    result: inout V
) where T : AccelerateBuffer, U : AccelerateBuffer, V : AccelerateMutableBuffer, T.Element == Float, U.Element == Float, V.Element == Float
```

## Parameters 

`vectorA`  

The first input vector, `A`.

`vectorB`  

The second input vector, `B`.

`result`  

The output vector, `C`.

## Discussion

This function calculates the division of the first `N` elements of input vectors `A` and `B`, and writes the result to output vector `C`.

```
 for (n = 0; n 

The following code shows an example of using this function:

```
    let count = 5

    let a: [Float] = [10, 20, 30, 40, 50]
    let b: [Float] = [ 1,  2,  3,  4,  5]

    let c = [Float](unsafeUninitializedCapacity: count) {
        buffer, initializedCount in

        vDSP.divide(a, b,
                    result: &buffer)

        initializedCount = count
    }

    // Prints "[10.0, 10.0, 10.0, 10.0, 10.0]".
    print(c)
```

## See Also

### Division

static func divide&lt;U>(Double, U) -> [Double]

Returns the double-precision element-wise division of a scalar value and a vector.

static func divide&lt;U>(U, Double) -> [Double]

Calculates the double-precision element-wise division of a vector and a scalar value.

static func divide&lt;T, U>(T, U) -> [Double]

Returns the double-precision element-wise division of two vectors.

static func divide&lt;U>(Float, U) -> [Float]

Returns the single-precision element-wise division of a scalar value and a vector.

static func divide&lt;U>(U, Float) -> [Float]

Calculates the single-precision element-wise division of a vector and a scalar value.

static func divide&lt;T, U>(T, U) -> [Float]

Returns the single-precision element-wise division of two vectors.

static func divide&lt;U, V>(Double, U, result: inout V)

Calculates the double-precision element-wise division of a scalar value and a vector.

static func divide&lt;U, V>(Float, U, result: inout V)

Calculates the single-precision element-wise division of a scalar value and a vector.

static func divide&lt;U, V>(U, Double, result: inout V)

Calculates the double-precision element-wise division of a vector and a scalar value.

static func divide&lt;U, V>(U, Float, result: inout V)

Calculates the single-precision element-wise division of a vector and a scalar value.

static func divide&lt;T, U, V>(T, U, result: inout V)

Calculates the double-precision element-wise division of two vectors.

static func divide(DSPSplitComplex, by: DSPSplitComplex, count: Int, result: inout DSPSplitComplex)

Calculates the single-precision elementwise division of a complex vector by a complex vector.

static func divide(DSPDoubleSplitComplex, by: DSPDoubleSplitComplex, count: Int, result: inout DSPDoubleSplitComplex)

Calculates the double-precision elementwise division of a complex vector by a complex vector.

static func divide&lt;U>(DSPSplitComplex, by: U, result: inout DSPSplitComplex)

Calculates the single-precision elementwise division of a complex vector by a real vector.

static func divide&lt;U>(DSPDoubleSplitComplex, by: U, result: inout DSPDoubleSplitComplex)

Calculates the double-precision elementwise division of a complex vector by a complex vector.

