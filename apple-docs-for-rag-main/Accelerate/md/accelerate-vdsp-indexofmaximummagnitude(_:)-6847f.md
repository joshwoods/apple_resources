

- Accelerate
- vDSP
-  indexOfMaximumMagnitude(\_:) 

Type Method

# indexOfMaximumMagnitude(\_:)

Returns the maximum magnitude and corresponding index in a double-precision vector.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func indexOfMaximumMagnitude(_ vector: U) -> (UInt, Double) where U : AccelerateBuffer, U.Element == Double
```

## Parameters 

`vector`  

The input vector.

## Return Value

A tuple that contains the maximum magnitude and corresponding index.

## Discussion

This function calculates the maximum magnitude and its corresponding index of the first `N` elements of the input vector and writes the results to the output scalar parameters, `C` and `I`, respectively.

The following code shows an example of using this function:

```
let a: [Double] = [-1.5, 2.25, 3.6,
                   0.2, -0.1, -4.3]

let indexOfMaximumMagnitude = vDSP.indexOfMaximumMagnitude(a)

// Prints "indexOfMaximumMagnitude (5, 4.3)".
print("indexOfMaximumMagnitude", indexOfMaximumMagnitude) 
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

