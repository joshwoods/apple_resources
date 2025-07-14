

- Accelerate
- vDSP
-  add(\_:\_:) 

Type Method

# add(\_:\_:)

Returns the single-precision element-wise sum of a vector and a scalar value.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func add(
    _ scalar: Float,
    _ vector: U
) -> [Float] where U : AccelerateBuffer, U.Element == Float
```

## Parameters 

`scalar`  

The input scalar value, `B`.

`vector`  

The input vector, `A`.

## Return Value

The output vector, `C`.

## Mentioned in 

Using vDSP for vector-based arithmetic

## Discussion

This function calculates the element-wise sum of vector `A` and scalar value `B`, and writes the result to vector `C`.

```
 for (n = 0; n 

The following code shows an example of using this function:

```
    let a: [Float] = [1, 2, 3, 4, 5]
    let b: Float = 10

    let c = vDSP.add(b, a)

    // Prints "[11.0, 22.0, 33.0, 44.0, 55.0]".
    print(c)
```

## See Also

### Addition

static func add&lt;U>(Double, U) -> [Double]

Returns the double-precision element-wise sum of a vector and a scalar value.

static func add&lt;T, U>(T, U) -> [Double]

Returns the double-precision element-wise sum of two vectors.

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

static func add&lt;T, U>(multiplication: (a: T, b: Float), U) -> [Float]

Returns the single-precision element-wise addition of the product of a vector and a scalar value, and a vector.

