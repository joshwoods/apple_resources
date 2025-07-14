

- Accelerate
- vDSP
-  linearInterpolate(values:atIndices:result:) 

Type Method

# linearInterpolate(values:atIndices:result:)

Computes the single-precision linearly interpolated values of a vector at the specified indices.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func linearInterpolate(
    values: T,
    atIndices indices: U,
    result: inout V
) where T : AccelerateBuffer, U : AccelerateBuffer, V : AccelerateMutableBuffer, T.Element == Float, U.Element == Float, V.Element == Float
```

## Parameters 

`values`  

The values to interpolate.

`indices`  

The indices to the output vector.

`result`  

The destination vector that receives the result.

## Discussion

The following code creates a five-element vector from two values using linear interpolation. The last index in `indices` determines the length of the operation result.

```
let values: [Float] = [0, 100]
let indices: [Float] = [0, 4]

let count = Int(indices.last!) + 1

let result = [Float](unsafeUninitializedCapacity: count) {
    buffer, initializedCount in

    vDSP.linearInterpolate(values: values,
                           atIndices: indices,
                           result: &buffer)

    initializedCount = count
}

// Prints "[0.0, 25.0, 50.0, 75.0, 100.0]".
print(result)
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

