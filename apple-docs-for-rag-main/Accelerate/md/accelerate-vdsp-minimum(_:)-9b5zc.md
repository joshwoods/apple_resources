

- Accelerate
- vDSP
-  minimum(\_:) 

Type Method

# minimum(\_:)

Returns the single-precision minimum value of a vector.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func minimum(_ vector: U) -> Float where U : AccelerateBuffer, U.Element == Float
```

## Parameters 

`vector`  

The input vector.

## Return Value

The minimum value of the vector.

## Discussion

This function calculates the minimum value of the first `N` elements of input vector `A`, and writes the result to output scalar `C`.

The following code shows an example of using this function:

```
let a: [Float] = [-1.5, 2.25, 3.6,
                  0.2, -0.1, -4.3]

let minimum = vDSP.minimum(a)
print("minimum", minimum) // Prints "minimum -4.3".
```

## See Also

### Type Methods

static func absolute&lt;U>(U) -> [Double]

Returns the absolute value of each element in the supplied double-precision vector.

static func absolute&lt;U>(U) -> [Float]

Returns the absolute value of each element in the supplied single-precision vector.

static func absolute&lt;V>(DSPSplitComplex, result: inout V)

Calculates the absolute value of each element in the supplied single-precision complex vector.

static func absolute&lt;V>(DSPDoubleSplitComplex, result: inout V)

Calculates the absolute value of each element in the supplied double-precision complex vector.

static func absolute&lt;U, V>(U, result: inout V)

Calculates the absolute value of each element in the supplied double-precision vector.

static func absolute&lt;U, V>(U, result: inout V)

Calculates the absolute value of each element in the supplied single-precision vector.

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

