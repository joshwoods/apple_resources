

- Accelerate
- vDSP
-  linearInterpolate(\_:\_:using:) 

Type Method

# linearInterpolate(\_:\_:using:)

Returns the linear interpolation between the supplied double-precision vectors.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func linearInterpolate(
    _ vectorA: T,
    _ vectorB: U,
    using interpolationConstant: Double
) -> [Double] where T : AccelerateBuffer, U : AccelerateBuffer, T.Element == Double, U.Element == Double
```

## Discussion

Single-precision and double-precision linearInterpolate(_:_:using:) functions return a vector that’s the elementwise linear interpolation between the two supplied vectors.

For example, the following code creates two arrays, vectorA and vectorB, that contain sine waves:

```
let n = 1024

let vectorA: [Float] = (0 ... n).map {
    return 2 + sin(Float($0) * 0.07)
}

let vectorB: [Float] = (0 ... n).map {
    return -2 + sin(Float($0) * 0.03)
}
```

Use linearInterpolate(_:_:using:) with an interpolation constant of 0.5 to generate a new vector that’s the average of the two sine waves:

```
let result = vDSP.linearInterpolate(vectorA, vectorB,
                                    using: 0.5)
```

The following figure visualizes the two source vectors: the blue lines at the top and bottom, and the interpolation result: the red line in the center:

## See Also

### Vector-to-Vector Linear Interpolation

static func linearInterpolate&lt;T, U>(T, U, using: Float) -> [Float]

Returns the linear interpolation between the supplied single-precision vectors.

static func linearInterpolate&lt;T, U, V>(T, U, using: Double, result: inout V)

Calculates the linear interpolation between the supplied double-precision vectors.

static func linearInterpolate&lt;T, U, V>(T, U, using: Float, result: inout V)

Calculates the linear interpolation between the supplied single-precision vectors.

