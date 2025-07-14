

- Accelerate
- vDSP
-  linearInterpolate(elementsOf:using:result:) 

Type Method

# linearInterpolate(elementsOf:using:result:)

Calculates the interpolation between the neighboring elements of a double-precision vector.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func linearInterpolate(
    elementsOf vector: T,
    using controlVector: U,
    result: inout V
) where T : AccelerateBuffer, U : AccelerateBuffer, V : AccelerateMutableBuffer, T.Element == Double, U.Element == Double, V.Element == Double
```

## Parameters 

`vector`  

An array that contains the values to interpolate.

`controlVector`  

An array that defines the interpolation: integer parts are indices into `vector` and fractional parts are interpolation constants.

`result`  

An array that receives the result of the calculation.

## Discussion

Single-precision and double-precision linearInterpolate(elementsOf:using:result:) functions calculate an array of an arbitrary length that’s constructed from the linearly interpolated values in a source array. Pass linearInterpolate(elementsOf:using:result:) a control vector that defines the interpolation: the integer part of each element in the control vector is the zero-based index of the first element of a pair of adjacent values in the source array, and the fractional part defines the linear interpolation between the values at those indices.

For example, the following code generates a five-element vector by interpolating three values:

```
let result = vDSP.linearInterpolate(elementsOf: [100, 200, 300],
                                    using: [0, 0.5, 1, 1.5, 2])
```

On return, `result` contains `[100.0, 150.0, 200.0, 250.0, 300.0]`.

To compute longer interpolation results, use ramp(in:count:) to generate the control vector. The following code creates 1024 interpolated values from 10 source values:

```
let values: [Float] = [50, 90, 55, 10, 40, 85, 65, 15, 30, 80]
let controlVector: [Float] = vDSP.ramp(in: 0 ... Float(values.count) - 1,
                                       count: 1024)

let result = vDSP.linearInterpolate(elementsOf: values,
                                    using: controlVector)
```

The following figure visualizes the elements in `result`.

By changing the technique used to form the fractional parts of the control vector, you change the interpolation between the values in the source vector. The following code uses a sigmoid function—that is, a function that has an “S” shaped curve—to populate the control vector:

```
let values: [Float] = [50, 90, 55, 10, 40, 85, 65, 15, 30, 80]

let denominator = 1024 / Float(values.count - 1)
let tau = Float.pi * 2
let controlVector: [Float] = (0 ..

The following figure visualizes the elements in `result` using hyperbolic tangent for the sigmoid function.

## See Also

### Single-Vector Linear Interpolation

Using linear interpolation to construct new data points

Fill the gaps in arrays of numerical data using linear interpolation.

static func linearInterpolate&lt;T, U>(elementsOf: T, using: U) -> [Double]

Returns the interpolation between the neighboring elements of a double-precision vector.

static func linearInterpolate&lt;T, U>(elementsOf: T, using: U) -> [Float]

Returns the interpolation between the neighboring elements of a single-precision vector.

static func linearInterpolate&lt;T, U, V>(elementsOf: T, using: U, result: inout V)

Calculates the interpolation between the neighboring elements of a single-precision vector.

