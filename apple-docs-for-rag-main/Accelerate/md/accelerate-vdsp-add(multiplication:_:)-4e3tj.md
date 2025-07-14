

- Accelerate
- vDSP
-  add(multiplication:\_:) 

Type Method

# add(multiplication:\_:)

Returns the double-precision element-wise addition of the product of a vector and a scalar value, and a vector.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func add(
    multiplication: (a: U, b: Double),
    _ scalar: Double
) -> [Double] where U : AccelerateBuffer, U.Element == Double
```

## Parameters 

`multiplication`  

A tuple that contains the vector `A` and the scalar value `B` in `D = (A * B) + C`.

`scalar`  

The input scalar value `C` in `D = (A * B) + C`.

## Return Value

The output vector `D` in `D = (A * B) + C`.

## Discussion

This function calculates the element-wise product of vector `A` and scalar value `B`, adds scalar value `C` to the product, and writes the result to vector `D`.

```
 for (n = 0; n 

The following code shows an example of using this function:

```
    let a: [Double] = [ 1,  2,  3,  4,  5]
    let b: Double = 10
    let c: Double = 5

    let d = vDSP.add(multiplication: (a, b),
                     c)

    // Prints "[15.0, 25.0, 35.0, 45.0, 55.0]".
    print(d)
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

static func add&lt;T, U>(multiplication: (a: T, b: Double), U) -> [Double]

Returns the double-precision element-wise addition of the product of a vector and a scalar value, and a vector.

static func add&lt;T, U>(multiplication: (a: T, b: U), Double) -> [Double]

Returns the double-precision element-wise sum of the product of two vectors, and a scalar value.

static func add&lt;S, T, U>(multiplication: (a: S, b: T), U) -> [Double]

Returns the double-precision element-wise sum of a vector and the product of two vectors.

static func add&lt;U>(multiplication: (a: U, b: Float), Float) -> [Float]

Returns the single-precision element-wise addition of the product of a vector and a scalar value, and a vector.

static func add&lt;T, U>(multiplication: (a: T, b: Float), U) -> [Float]

Returns the single-precision element-wise addition of the product of a vector and a scalar value, and a vector.

