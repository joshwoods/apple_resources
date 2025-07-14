

- Accelerate
- vDSP
-  formStereoRamp(withInitialValue:multiplyingBy:\_:increment:results:\_:) 

Type Method

# formStereoRamp(withInitialValue:multiplyingBy:\_:increment:results:\_:)

Populates two single-precision vectors that contain stereo monotonically incrementing or decrementing values multiplied by two source vectors.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func formStereoRamp(
    withInitialValue initialValue: inout Float,
    multiplyingBy multiplierOne: U,
    _ multiplierTwo: U,
    increment: Float,
    results resultOne: inout V,
    _ resultTwo: inout V
) where U : AccelerateBuffer, V : AccelerateMutableBuffer, U.Element == Float, V.Element == Float
```

## Parameters 

`initialValue`  

The initial value of the ramp.

`multiplierOne`  

The first input vector that’s multiplied by the ramp function.

`multiplierTwo`  

The second input vector that’s multiplied by the ramp function.

`increment`  

The increment, or decrement if negative, between each generated element.

`resultOne`  

The increment, or decrement if negative, between each generated element.

`resultTwo`  

The array to overwrite with the first generated ramp.

## Discussion

Use this function to populate two vectors by multiplying the values in two input vectors with the corresponding values of a ramp.

For example, the following code fills the arrays `multiplierOne` and `multiplierTwo` with sine values:

```
let n = vDSP_Length(1024)

let multiplierOne: [Float] = (0 ..

The following figure illustrates the values of `multiplierOne`, as a solid line, and `multiplierTwo`, as a dashed line:

Pass `multiplierOne` and `multiplierTwo` as the `multiplyingBy` parameter of formStereoRamp(withInitialValue:multiplyingBy:_:increment:results:_:):

```
var start: Float = 0
let step: Float = 0.1

var resultOne = [Float](repeating: 0,
                count: Int(n))
var resultTwo = [Float](repeating: 0,
                count: Int(n))

vDSP.formStereoRamp(withInitialValue: &start,
                    multiplyingBy: multiplierOne, multiplierTwo,
                    increment: step,
                    results: &resultOne, &resultTwo)
```

On return, the output vectors, `results.firstOutput` and `results.secondOutput`, contain ramped-sine waves. The figure below shows the first output as a solid line and the second output as a dashed line:

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

