

- Accelerate
- vDSP
-  hypot(\_:\_:result:) 

Type Method

# hypot(\_:\_:result:)

Calculates the single-precision hypotenuses of right triangles with legs that are the lengths of corresponding elements of the two input vectors.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func hypot(
    _ x: T,
    _ y: U,
    result: inout V
) where T : AccelerateBuffer, U : AccelerateBuffer, V : AccelerateMutableBuffer, T.Element == Float, U.Element == Float, V.Element == Float
```

## Parameters 

`x`  

An array that contains the lengths of the first set of legs of the triangles.

`y`  

An array that contains the lengths of the second set of legs of the triangles.

`result`  

An array that receives the result of the calculation.

## Discussion

This function calculates the square roots of the sum of the squares of corresponding elements of vectors `x` and `y`, using the following operation:

```
for (n = 0; n 

For example, the following code calculates the hypotenuse of four Pythagorean triples:

```
    let x: [Float] = [3, 6, 5, 9]
    let y: [Float] = [4, 8, 12, 12]

    let hypotenuses = [Float](
        unsafeUninitializedCapacity: x.count) {
            buffer, initializedCount in

            vDSP.hypot(x, y,
                       result: &buffer)

            initializedCount = x.count
        }

    // Prints "[5.0, 10.0, 13.0, 15.0]".
    print(hypotenuses)
```

## See Also

### Related Documentation

vDSP_vdist

Calculates the single-precision hypotenuses of right triangles with legs that are the lengths of corresponding elements of two pairs of vectors.

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

