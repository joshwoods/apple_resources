

- Accelerate
- vDSP
-  formRamp(withInitialValue:increment:result:) 

Type Method

# formRamp(withInitialValue:increment:result:)

Populates a single-precision vector with monotonically incrementing or decrementing values using an initial value and increment.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func formRamp(
    withInitialValue initialValue: Float,
    increment: Float,
    result: inout V
) where V : AccelerateMutableBuffer, V.Element == Float
```

## Parameters 

`initialValue`  

The initial value of the ramp.

`increment`  

The increment, or decrement if negative, between each generated element.

`result`  

The array that receives the generated ramp.

## Discussion

Use this function to generate and return a vector populated with ramped values.

The following code generates a ramped vector with values in the range `0 ... 7`:

```
    let n = 8

    let ramp = [Float](unsafeUninitializedCapacity: n) {
        buffer, initializedCount in

        vDSP.formRamp(withInitialValue: 0,
                      increment: 1,
                      result: &buffer)

        initializedCount = n
    }

    // Prints "[0.0, 1.0, 2.0, 3.0, 4.0, 5.0, 6.0, 7.0]".
    print(ramp)
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

