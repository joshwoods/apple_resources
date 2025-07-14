

- Accelerate
- vDSP
-  add(multiplication:multiplication:) 

Type Method

# add(multiplication:multiplication:)

Returns the double-precision element-wise addition of two vector-scalar products.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func add(
    multiplication multiplicationAB: (a: T, b: Double),
    multiplication multiplicationCD: (c: U, d: Double)
) -> [Double] where T : AccelerateBuffer, U : AccelerateBuffer, T.Element == Double, U.Element == Double
```

## Parameters 

`multiplicationAB`  

A tuple that contains the vector `A` and the scalar value `B` in `E = (A * B) + (C * D)`.

`multiplicationCD`  

A tuple that contains the vector `C` and the scalar value `D` in `E = (A * B) + (C * D)`.

## Return Value

The output vector `E` in `E = (A * B) + (C * D)`.

## Discussion

This function calculates the element-wise vector-scalar products of `A` and `B`, and `C` and `D`, and writes the sum of the products to vector `D`.

```
for (n = 0; n 

The following code shows an example of using this function:

```
    let count = 5

    let a: [Double] = [ 1,  2,  3,  4,  5]
    let b: Double = 10
    let c: [Double] = [ 5,  4,  3,  2,  1]
    let d: Double = 50

    let e = vDSP.add(multiplication: (a, b),
                     multiplication: (c, d))

    // Prints "[260.0, 220.0, 180.0, 140.0, 100.0]".
    print(e)
```

## See Also

### Addition

static func add&lt;U>(Double, U) -> [Double]

Returns the double-precision element-wise sum of a vector and a scalar value.

static func add&lt;T, U>(T, U) -> [Double]

Returns the double-precision element-wise sum of two vectors.

static func add&lt;U>(Float, U) -> [Float]

Returns the single-precision element-wise sum of a vector and a scalar value.

static func add&lt;T, U>(T, U) -> [Float]

Returns the single-precision element-wise sum of two vectors.

static func add&lt;U, V>(Double, U, result: inout V)

Calculates the single-precision element-wise sum of a vector and a scalar value.

static func add&lt;U, V>(Float, U, result: inout V)

Calculates the single-precision element-wise sum of a vector and a scalar value.

static func add&lt;T, U, V>(T, U, result: inout V)

Calculates the double-precision element-wise sum of two vectors.

static func add&lt;T, U, V>(T, U, result: inout V)

Calculates the single-precision element-wise sum of two vectors.

static func add(DSPSplitComplex, to: DSPSplitComplex, count: Int, result: inout DSPSplitComplex)

Calculates the single-precision elementwise sum of the supplied complex vectors.

static func add(DSPDoubleSplitComplex, to: DSPDoubleSplitComplex, count: Int, result: inout DSPDoubleSplitComplex)

Calculates the double-precision elementwise sum of the supplied complex vectors.

static func add&lt;U>(multiplication: (a: U, b: Double), Double) -> [Double]

Returns the double-precision element-wise addition of the product of a vector and a scalar value, and a vector.

static func add&lt;T, U>(multiplication: (a: T, b: Double), U) -> [Double]

Returns the double-precision element-wise addition of the product of a vector and a scalar value, and a vector.

static func add&lt;T, U>(multiplication: (a: T, b: U), Double) -> [Double]

Returns the double-precision element-wise sum of the product of two vectors, and a scalar value.

static func add&lt;S, T, U>(multiplication: (a: S, b: T), U) -> [Double]

Returns the double-precision element-wise sum of a vector and the product of two vectors.

static func add&lt;U>(multiplication: (a: U, b: Float), Float) -> [Float]

Returns the single-precision element-wise addition of the product of a vector and a scalar value, and a vector.

