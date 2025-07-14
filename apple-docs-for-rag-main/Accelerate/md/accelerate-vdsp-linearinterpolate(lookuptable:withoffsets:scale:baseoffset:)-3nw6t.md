

- Accelerate
- vDSP
-  linearInterpolate(lookupTable:withOffsets:scale:baseOffset:) 

Type Method

# linearInterpolate(lookupTable:withOffsets:scale:baseOffset:)

Returns the single-precision linearly interpolated values of a lookup table from the specified offsets.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func linearInterpolate(
    lookupTable: T,
    withOffsets offsets: U,
    scale: Float = 1,
    baseOffset: Float = 0
) -> [Float] where T : AccelerateBuffer, U : AccelerateBuffer, T.Element == Float, U.Element == Float
```

## Parameters 

`lookupTable`  

The lookup table.

`offsets`  

The offsets into the lookup table.

`scale`  

The scale factor for the offsets.

`baseOffset`  

The base offset for the offsets.

## Return Value

The result of the interpolation operation.

## Discussion

The following code shows the result of linearly interpolating a lookup table that contains the values `[-10, 0, 100]` using the offsets `[0, 0.5, 1, 1.5, 2]`. The integer offsets, `0`, `1`, and `2`, return the corresponding values in the lookup table, `-10`, `0`, and `2`. The noninteger offsets, `0.5` and `1.5`, return the linearly interpolated values between the lookup table values, `-5` and `50`.

```
let lookupTable: [Float] = [-10, 0, 100]
let offsets: [Float] = [0, 0.5, 1, 1.5, 2]

let result = vDSP.linearInterpolate(lookupTable: lookupTable,
                                    withOffsets: offsets)

// Prints "[-10.0, -5.0, 0.0, 50.0, 100.0]".
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

