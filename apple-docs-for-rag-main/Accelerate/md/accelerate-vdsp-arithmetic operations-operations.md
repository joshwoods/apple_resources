

- Accelerate
- vDSP
-  Arithmetic operations 

API Collection

# Arithmetic operations

Perform operations on large vectors.

## Topics

### Addition

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

static func add(DSPDoubleSplitComplex, to: DSPDoubleSplitComplex, count: Int, result: inout DSPDoubleSplitComplex)

Calculates the double-precision elementwise sum of the supplied complex vectors.

static func add&lt;U>(multiplication: (a: U, b: Double), Double) -> [Double]

Returns the double-precision element-wise addition of the product of a vector and a scalar value, and a vector.

static func add&lt;T, U>(multiplication: (a: T, b: Double), U) -> [Double]

Returns the double-precision element-wise addition of the product of a vector and a scalar value, and a vector.

static func add&lt;T, U>(multiplication: (a: T, b: U), Double) -> [Double]

Returns the double-precision element-wise sum of the product of two vectors, and a scalar value.

static func add&lt;S, T, U>(multiplication: (a: S, b: T), U) -> [Double]

Returns the double-precision element-wise sum of a vector and the product of two vectors.

static func add&lt;U>(multiplication: (a: U, b: Float), Float) -> [Float]

Returns the single-precision element-wise addition of the product of a vector and a scalar value, and a vector.

static func add&lt;T, U>(multiplication: (a: T, b: Float), U) -> [Float]

Returns the single-precision element-wise addition of the product of a vector and a scalar value, and a vector.

static func add&lt;T, U>(multiplication: (a: T, b: U), Float) -> [Float]

Returns the single-precision element-wise sum of the product of two vectors, and a scalar value.

static func add&lt;S, T, U>(multiplication: (a: S, b: T), U) -> [Float]

Returns the single-precision element-wise sum of a vector and the product of two vectors.

static func add&lt;U, V>(multiplication: (a: U, b: Double), Double, result: inout V)

Calculates the double-precision element-wise addition of the product of a vector and a scalar value, and a vector.

static func add&lt;T, U, V>(multiplication: (a: T, b: Double), U, result: inout V)

Calculates the double-precision element-wise addition of the product of a vector and a scalar value, and a vector.

static func add&lt;U, V>(multiplication: (a: U, b: Float), Float, result: inout V)

Calculates the single-precision element-wise addition of the product of a vector and a scalar value, and a vector.

static func add&lt;T, U, V>(multiplication: (a: T, b: Float), U, result: inout V)

Calculates the single-precision element-wise addition of the product of a vector and a scalar value, and a vector.

static func add&lt;T, U, V>(multiplication: (a: T, b: U), Double, result: inout V)

Calculates the double-precision element-wise sum of the product of two vectors, and a scalar value.

static func add&lt;T, U, V>(multiplication: (a: T, b: U), Float, result: inout V)

Calculates the single-precision element-wise sum of the product of two vectors, and a scalar value.

static func add&lt;S, T, U, V>(multiplication: (a: S, b: T), U, result: inout V)

Calculates the double-precision element-wise sum of a vector and the product of two vectors.

static func add&lt;S, T, U, V>(multiplication: (a: S, b: T), U, result: inout V)

Calculates the single-precision element-wise sum of a vector and the product of two vectors.

static func add&lt;T, U>(multiplication: (a: T, b: Double), multiplication: (c: U, d: Double)) -> [Double]

Returns the double-precision element-wise addition of two vector-scalar products.

static func add&lt;R, S, T, U>(multiplication: (a: R, b: S), multiplication: (c: T, d: U)) -> [Double]

Returns the double-precision elementwise product of a vector and a vector, added to a second product of a vector and a vector.

static func add&lt;T, U>(multiplication: (a: T, b: Float), multiplication: (c: U, d: Float)) -> [Float]

Returns the single-precision element-wise addition of two vector-scalar products.

static func add&lt;R, S, T, U>(multiplication: (a: R, b: S), multiplication: (c: T, d: U)) -> [Float]

Returns the single-precision elementwise product of a vector and a vector, added to a second product of a vector and a vector.

static func add&lt;T, U, V>(multiplication: (a: T, b: Double), multiplication: (c: U, d: Double), result: inout V)

Calculates the double-precision element-wise addition of two vector-scalar products.

static func add&lt;T, U, V>(multiplication: (a: T, b: Float), multiplication: (c: U, d: Float), result: inout V)

Calculates the single-precision element-wise addition of two vector-scalar products.

static func add&lt;R, S, T, U, V>(multiplication: (a: R, b: S), multiplication: (c: T, d: U), result: inout V)

Calculates the double-precision elementwise product of a vector and a vector, added to a second product of a vector and a vector.

static func add&lt;R, S, T, U, V>(multiplication: (a: R, b: S), multiplication: (c: T, d: U), result: inout V)

Calculates the single-precision elementwise product of a vector and a vector, added to a second product of a vector and a vector.

### Subtraction

static func subtract&lt;T, U>(U, T) -> [Double]

Returns the double-precision element-wise subtraction of two vectors.

static func subtract&lt;T, U>(U, T) -> [Float]

Returns the single-precision element-wise subtraction of two vectors.

static func subtract&lt;T, U, V>(U, T, result: inout V)

Calculates the double-precision element-wise subtraction of two vectors.

static func subtract&lt;T, U, V>(U, T, result: inout V)

Calculates the single-precision element-wise subtraction of two vectors.

static func subtract(DSPSplitComplex, from: DSPSplitComplex, count: Int, result: inout DSPSplitComplex)

Calculates the single-precision elementwise subtraction of a complex vector from a complex vector.

static func subtract(DSPDoubleSplitComplex, from: DSPDoubleSplitComplex, count: Int, result: inout DSPDoubleSplitComplex)

Calculates the double-precision elementwise subtraction of a complex vector from a complex vector.

static func subtract&lt;T, U>(multiplication: (a: U, b: Double), T) -> [Double]

Calculates the double-precision element-wise difference of the product of a vector and a scalar value, and a vector.

static func subtract&lt;S, T, U>(multiplication: (a: T, b: U), S) -> [Double]

Returns the double-precision element-wise difference of a vector and the product of two vectors.

static func subtract&lt;T, U>(multiplication: (a: U, b: Float), T) -> [Float]

Calculates the single-precision element-wise difference of the product of a vector and a scalar value, and a vector.

static func subtract&lt;S, T, U>(multiplication: (a: T, b: U), S) -> [Float]

Returns the single-precision element-wise difference of a vector and the product of two vectors.

static func subtract&lt;T, U, V>(multiplication: (a: U, b: Double), T, result: inout V)

Calculates the double-precision element-wise difference of the product of a vector and a scalar value, and a vector.

static func subtract&lt;T, U, V>(multiplication: (a: U, b: Float), T, result: inout V)

Calculates the single-precision element-wise difference of the product of a vector and a scalar value, and a vector.

static func subtract&lt;S, T, U, V>(multiplication: (a: T, b: U), S, result: inout V)

Calculates the double-precision element-wise difference of a vector and the product of two vectors.

static func subtract&lt;S, T, U, V>(multiplication: (a: T, b: U), S, result: inout V)

Calculates the single-precision element-wise difference of a vector and the product of two vectors.

static func subtract&lt;R, S, T, U>(multiplication: (a: T, b: U), multiplication: (c: R, d: S)) -> [Double]

Returns the double-precision element-wise difference of the products of two pairs of vectors.

static func subtract&lt;R, S, T, U>(multiplication: (a: T, b: U), multiplication: (c: R, d: S)) -> [Float]

Returns the single-precision element-wise difference of the products of two pairs of vectors.

static func subtract&lt;R, S, T, U, V>(multiplication: (a: T, b: U), multiplication: (c: R, d: S), result: inout V)

Calculates the double-precision element-wise difference of the products of two pairs of vectors.

static func subtract&lt;R, S, T, U, V>(multiplication: (a: T, b: U), multiplication: (c: R, d: S), result: inout V)

Calculates the single-precision element-wise difference of the products of two pairs of vectors.

### Addition and Subtraction

static func addSubtract&lt;S, T, U, V>(S, T, addResult: inout U, subtractResult: inout V)

Calculates the double-precision element-wise sum and subtraction of two vectors.

static func addSubtract&lt;S, T, U, V>(S, T, addResult: inout U, subtractResult: inout V)

Calculates the single-precision element-wise sum and subtraction of two vectors.

### Multiplication

static func multiply&lt;U>(Double, U) -> [Double]

Returns the double-precision element-wise product of a vector and a scalar value.

static func multiply&lt;T, U>(T, U) -> [Double]

Returns the double-precision element-wise product of two vectors.

static func multiply&lt;U>(Float, U) -> [Float]

Returns the single-precision element-wise product of a vector and a scalar value.

static func multiply&lt;T, U>(T, U) -> [Float]

Returns the single-precision element-wise product of two vectors.

static func multiply&lt;U, V>(Double, U, result: inout V)

Calculates the double-precision element-wise product of a vector and a scalar value.

static func multiply&lt;U, V>(Float, U, result: inout V)

Calculates the single-precision element-wise product of a vector and a scalar value.

static func multiply&lt;T, U, V>(T, U, result: inout V)

Calculates the double-precision element-wise product of two vectors.

static func multiply&lt;T, U, V>(T, U, result: inout V)

Calculates the single-precision element-wise product of two vectors.

static func multiply(DSPSplitComplex, by: DSPSplitComplex, count: Int, useConjugate: Bool, result: inout DSPSplitComplex)

Calculates the product of two complex single-precision vectors, optionally conjugating one of them.

static func multiply(DSPDoubleSplitComplex, by: DSPDoubleSplitComplex, count: Int, useConjugate: Bool, result: inout DSPDoubleSplitComplex)

Calculates the elementwise product of two complex double-precision vectors, optionally conjugating one of them.

static func multiply&lt;U>(DSPSplitComplex, by: U, result: inout DSPSplitComplex)

Calculates the double-precision elementwise product of a complex vector and a real vector.

static func multiply&lt;U>(DSPDoubleSplitComplex, by: U, result: inout DSPDoubleSplitComplex)

Calculates the single-precision elementwise product of a complex vector and a real vector.

static func multiply&lt;T, U>(addition: (a: T, b: U), Double) -> [Double]

Returns the double-precision element-wise product of the sum of two vectors and a scalar value.

static func multiply&lt;S, T, U>(addition: (a: S, b: T), U) -> [Double]

Returns the double-precision element-wise product of a vector and the sum of two vectors.

static func multiply&lt;T, U>(addition: (a: T, b: U), Float) -> [Float]

Returns the single-precision element-wise product of the sum of two vectors and a scalar value.

static func multiply&lt;S, T, U>(addition: (a: S, b: T), U) -> [Float]

Returns the single-precision element-wise product of a vector and the sum of two vectors.

static func multiply&lt;T, U, V>(addition: (a: T, b: U), Double, result: inout V)

Calculates the double-precision element-wise product of the sum of two vectors and a scalar value.

static func multiply&lt;T, U, V>(addition: (a: T, b: U), Float, result: inout V)

Calculates the single-precision element-wise product of the sum of two vectors and a scalar value.

static func multiply&lt;S, T, U, V>(addition: (a: S, b: T), U, result: inout V)

Calculates the double-precision element-wise product of a vector and the sum of two vectors.

static func multiply&lt;S, T, U, V>(addition: (a: S, b: T), U, result: inout V)

Calculates the single-precision element-wise product of a vector and the sum of two vectors.

static func multiply&lt;S, T, U>(addition: (a: S, b: T), addition: (c: U, d: U)) -> [Double]

Returns the double-precision element-wise product of the sums of two pairs of vectors.

static func multiply&lt;S, T, U>(addition: (a: S, b: T), addition: (c: U, d: U)) -> [Float]

Returns the single-precision element-wise product of the sums of two pairs of vectors.

static func multiply&lt;S, T, U, V>(addition: (a: S, b: T), addition: (c: U, d: U), result: inout V)

Calculates the double-precision element-wise product of the sums of two pairs of vectors.

static func multiply&lt;S, T, U, V>(addition: (a: S, b: T), addition: (c: U, d: U), result: inout V)

Calculates the single-precision element-wise product of the sums of two pairs of vectors.

static func multiply&lt;R, S, T, U>(addition: (a: R, b: S), subtraction: (c: T, d: U)) -> [Double]

Returns the double-precision element-wise product of the sum of two vectors and the difference of two vectors.

static func multiply&lt;R, S, T, U>(addition: (a: R, b: S), subtraction: (c: T, d: U)) -> [Float]

Returns the single-precision element-wise product of the sum of two vectors and the difference of two vectors.

static func multiply&lt;R, S, T, U, V>(addition: (a: R, b: S), subtraction: (c: T, d: U), result: inout V)

Calculates the double-precision element-wise product of the sum of two vectors and the difference of two vectors.

static func multiply&lt;R, S, T, U, V>(addition: (a: R, b: S), subtraction: (c: T, d: U), result: inout V)

Calculates the double-precision element-wise product of the sum of two vectors and the difference of two vectors.

static func multiply&lt;T, U>(subtraction: (a: T, b: U), Double) -> [Double]

Returns the double-precision element-wise product of the difference of two vectors and a scalar value.

static func multiply&lt;S, T, U>(subtraction: (a: S, b: T), U) -> [Double]

Returns the double-precision element-wise product of a vector and the differences of two vectors.

static func multiply&lt;T, U>(subtraction: (a: T, b: U), Float) -> [Float]

Returns the single-precision element-wise product of the difference of two vectors and a scalar value.

static func multiply&lt;S, T, U>(subtraction: (a: S, b: T), U) -> [Float]

Returns the single-precision element-wise product of a vector and the differences of two vectors.

static func multiply&lt;T, U, V>(subtraction: (a: T, b: U), Double, result: inout V)

Calculates the double-precision element-wise product of the difference of two vectors and a scalar value.

static func multiply&lt;T, U, V>(subtraction: (a: T, b: U), Float, result: inout V)

Calculates the single-precision element-wise product of the difference of two vectors and a scalar value.

static func multiply&lt;S, T, U, V>(subtraction: (a: S, b: T), U, result: inout V)

Calculates the double-precision element-wise product of a vector and the differences of two vectors.

static func multiply&lt;S, T, U, V>(subtraction: (a: S, b: T), U, result: inout V)

Calculates the single-precision element-wise product of a vector and the differences of two vectors.

static func multiply&lt;R, S, T, U>(subtraction: (a: R, b: S), subtraction: (c: T, d: U)) -> [Double]

Returns the double-precision element-wise product of the differences of two pairs of vectors.

static func multiply&lt;R, S, T, U>(subtraction: (a: R, b: S), subtraction: (c: T, d: U)) -> [Float]

Returns the single-precision element-wise product of the differences of two pairs of vectors.

static func multiply&lt;R, S, T, U, V>(subtraction: (a: R, b: S), subtraction: (c: T, d: U), result: inout V)

Calculates the double-precision element-wise product of the differences of two pairs of vectors.

static func multiply&lt;R, S, T, U, V>(subtraction: (a: R, b: S), subtraction: (c: T, d: U), result: inout V)

Calculates the single-precision element-wise product of the differences of two pairs of vectors.

### Division

static func divide&lt;U>(Double, U) -> [Double]

Returns the double-precision element-wise division of a scalar value and a vector.

static func divide&lt;U>(U, Double) -> [Double]

Calculates the double-precision element-wise division of a vector and a scalar value.

static func divide&lt;T, U>(T, U) -> [Double]

Returns the double-precision element-wise division of two vectors.

static func divide&lt;U>(Float, U) -> [Float]

Returns the single-precision element-wise division of a scalar value and a vector.

static func divide&lt;U>(U, Float) -> [Float]

Calculates the single-precision element-wise division of a vector and a scalar value.

static func divide&lt;T, U>(T, U) -> [Float]

Returns the single-precision element-wise division of two vectors.

static func divide&lt;U, V>(Double, U, result: inout V)

Calculates the double-precision element-wise division of a scalar value and a vector.

static func divide&lt;U, V>(Float, U, result: inout V)

Calculates the single-precision element-wise division of a scalar value and a vector.

static func divide&lt;U, V>(U, Double, result: inout V)

Calculates the double-precision element-wise division of a vector and a scalar value.

static func divide&lt;U, V>(U, Float, result: inout V)

Calculates the single-precision element-wise division of a vector and a scalar value.

static func divide&lt;T, U, V>(T, U, result: inout V)

Calculates the double-precision element-wise division of two vectors.

static func divide&lt;T, U, V>(T, U, result: inout V)

Calculates the single-precision element-wise division of two vectors.

static func divide(DSPSplitComplex, by: DSPSplitComplex, count: Int, result: inout DSPSplitComplex)

Calculates the single-precision elementwise division of a complex vector by a complex vector.

static func divide(DSPDoubleSplitComplex, by: DSPDoubleSplitComplex, count: Int, result: inout DSPDoubleSplitComplex)

Calculates the double-precision elementwise division of a complex vector by a complex vector.

static func divide&lt;U>(DSPSplitComplex, by: U, result: inout DSPSplitComplex)

Calculates the single-precision elementwise division of a complex vector by a real vector.

static func divide&lt;U>(DSPDoubleSplitComplex, by: U, result: inout DSPDoubleSplitComplex)

Calculates the double-precision elementwise division of a complex vector by a complex vector.

