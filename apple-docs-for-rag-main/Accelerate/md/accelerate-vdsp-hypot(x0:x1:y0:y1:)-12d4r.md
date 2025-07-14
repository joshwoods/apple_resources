

- Accelerate
- vDSP
-  hypot(x0:x1:y0:y1:) 

Type Method

# hypot(x0:x1:y0:y1:)

Returns the double-precision hypotenuses of right triangles with legs that are the differences of corresponding elements of two pairs of vectors.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func hypot(
    x0: R,
    x1: S,
    y0: T,
    y1: U
) -> [Double] where R : AccelerateBuffer, S : AccelerateBuffer, T : AccelerateBuffer, U : AccelerateBuffer, R.Element == Double, S.Element == Double, T.Element == Double, U.Element == Double
```

## Parameters 

`x0`  

An array that contains the first values of the first set of legs of the triangles.

`x1`  

An array that contains the second values of the first set of legs of the triangles.

`y0`  

An array that contains the first values of the second set of legs of the triangles.

`y1`  

An array that contains the second values of the second set of legs of the triangles.

## Discussion

This function returns the length of the hypotenuse of *n* number of triangles, where *n* is the number of elements in the supplied vectors. The differences between corresponding elements of vectors `x0` and `x1` and vectors `y0` and `y1` define the lengths of the two legs of each triangle.

The functions use the following operation:

```
for (n = 0; n 

For example, the following code calculates the hypotenuse of four Pythagorean triples:

```
    let x0: [Double] = [3, 6, 5, 9]
    let x1: [Double] = [0, 0, 0, 0]

    let y0: [Double] = [0, 0, 0, 0]
    let y1: [Double] = [4, 8, 12, 12]

    let hypotenuses = vDSP.hypot(x0: x0, x1: x1,
                                 y0: y0, y1: y1)

    // Prints "[5.0, 10.0, 13.0, 15.0]".
    print(hypotenuses)
```

## See Also

### Related Documentation

vDSP_vpythg

Calculates the single-precision hypotenuses of right triangles with legs that are the differences of corresponding elements of two pairs of vectors.

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

