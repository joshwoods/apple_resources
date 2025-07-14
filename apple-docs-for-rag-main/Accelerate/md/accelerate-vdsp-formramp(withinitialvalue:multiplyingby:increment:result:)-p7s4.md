

- Accelerate
- vDSP
-  formRamp(withInitialValue:multiplyingBy:increment:result:) 

Type Method

# formRamp(withInitialValue:multiplyingBy:increment:result:)

Populates a double-precision vector that contains monotonically incrementing or decrementing values, and multiplies that vector by a source vector.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func formRamp(
    withInitialValue initialValue: inout Double,
    multiplyingBy vector: U,
    increment: Double,
    result: inout V
) where U : AccelerateBuffer, V : AccelerateMutableBuffer, U.Element == Double, V.Element == Double
```

## Parameters 

`initialValue`  

On input, the initial value of the ramp. On output, the next value in the ramp.

`vector`  

The input vector that the function multiplies by the ramp.

`increment`  

The increment, or decrement if negative, between each generated element.

`result`  

The result.

## Discussion

Use this function to generate and return a vector populated with ramped values with each element multiplied by the corresponding element in a second vector.

The following code generates a ramped vector with values in the range `0 ... 7`. The function multiplies elements at even indices by `10` and multiplies elements at odd indices by `100`.

```
    let n = 8

    var initialValue: Double = 0
    let increment: Double = 1

    let ramp = [Double](unsafeUninitializedCapacity: n) {
        buffer, initializedCount in

        vDSP.formRamp(withInitialValue: &initialValue,
                      multiplyingBy: [10, 100, 10, 100, 10, 100, 10, 100],
                      increment: increment,
                      result: &buffer)

        initializedCount = n
    }

    // Prints "[0.0, 100.0, 20.0, 300.0, 40.0, 500.0, 60.0, 700.0]".
    print(ramp)

    // Prints "8".
    print(initialValue)
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

