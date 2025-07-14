

- Accelerate
- vDSP
-  distanceSquared(\_:\_:) 

Type Method

# distanceSquared(\_:\_:)

Returns the double-precision distance squared between two points in n-dimensional space.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
static func distanceSquared(
    _ pointA: U,
    _ pointB: V
) -> Double where U : AccelerateBuffer, V : AccelerateMutableBuffer, U.Element == Double, V.Element == Double
```

## Parameters 

`pointA`  

An array that contains the coordinates of the first point.

`pointB`  

An array that contains the coordinates of the second point.

## Discussion

This function calculates the sum of squares of the differences of corresponding elements of vectors `A` and `B`, using the following operation:

```
C[0] = sum((A[n] - B[n]) ** 2, 0 

For example, the following code calculates the distance squared between the two four-dimensional points `pointA` and `pointB`:

```
    let pointA: [Double] = [-1, 0, -2, 1]
    let pointB: [Double] = [ 2, 1,  4, 3]

    let distanceSquared = vDSP.distanceSquared(pointA, pointB)

    print("distance²", distanceSquared) // Prints "distance² 50.0".
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

