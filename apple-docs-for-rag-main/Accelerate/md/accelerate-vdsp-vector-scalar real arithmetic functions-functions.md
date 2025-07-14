

- Accelerate
- vDSP
-  Vector-scalar real arithmetic functions 

API Collection

# Vector-scalar real arithmetic functions

Perform element-wise operations on combinations of vectors of real values and scalar values.

## Overview

The vDSP library provides a suite of general-purpose, high-performance arithmetic functions that are alternatives to `for` loops and `map` when you apply operations on collections of floating-point values.

See Using vDSP for vector-based arithmetic for a summary of available operations.

## Topics

### Vector-scalar addition operations

static func add&lt;U>(Float, U) -> [Float]

Returns the single-precision element-wise sum of a vector and a scalar value.

static func add&lt;U>(Double, U) -> [Double]

Returns the double-precision element-wise sum of a vector and a scalar value.

static func add&lt;U, V>(Float, U, result: inout V)

Calculates the single-precision element-wise sum of a vector and a scalar value.

static func add&lt;U, V>(Double, U, result: inout V)

Calculates the single-precision element-wise sum of a vector and a scalar value.

vDSP_vsaddi

Calculates the integer element-wise sum of a vector and a scalar value, using the specified stride.

vDSP_vsadd

Calculates the single-precision element-wise sum of a vector and a scalar value, using the specified stride.

vDSP_vsaddD

Calculates the double-precision element-wise sum of a vector and a scalar value, using the specified stride.

### Vector-scalar multiplication operations

static func multiply&lt;U>(Float, U) -> [Float]

Returns the single-precision element-wise product of a vector and a scalar value.

static func multiply&lt;U>(Double, U) -> [Double]

Returns the double-precision element-wise product of a vector and a scalar value.

static func multiply&lt;U, V>(Float, U, result: inout V)

Calculates the single-precision element-wise product of a vector and a scalar value.

static func multiply&lt;U, V>(Double, U, result: inout V)

Calculates the double-precision element-wise product of a vector and a scalar value.

vDSP_vsmul

Calculates the single-precision element-wise product of a vector and a scalar value, using the specified stride.

vDSP_vsmulD

Calculates the double-precision element-wise product of a vector and a scalar value, using the specified stride.

### Vector-scalar division operations

static func divide&lt;U>(U, Float) -> [Float]

Calculates the single-precision element-wise division of a vector and a scalar value.

static func divide&lt;U>(U, Double) -> [Double]

Calculates the double-precision element-wise division of a vector and a scalar value.

static func divide&lt;U, V>(U, Float, result: inout V)

Calculates the single-precision element-wise division of a vector and a scalar value.

static func divide&lt;U, V>(U, Double, result: inout V)

Calculates the double-precision element-wise division of a vector and a scalar value.

vDSP_vsdivi

Calculates the integer element-wise division of a vector and a scalar value, using the specified stride.

vDSP_vsdiv

Calculates the single-precision element-wise division of a vector and a scalar value, using the specified stride.

vDSP_vsdivD

Calculates the double-precision element-wise division of a vector and a scalar value, using the specified stride.

### Scalar-vector division operations

static func divide&lt;U>(Float, U) -> [Float]

Returns the single-precision element-wise division of a scalar value and a vector.

static func divide&lt;U>(Double, U) -> [Double]

Returns the double-precision element-wise division of a scalar value and a vector.

static func divide&lt;U, V>(Float, U, result: inout V)

Calculates the single-precision element-wise division of a scalar value and a vector.

static func divide&lt;U, V>(Double, U, result: inout V)

Calculates the double-precision element-wise division of a scalar value and a vector.

vDSP_svdiv

Calculates the single-precision element-wise division of a scalar value and a vector, using the specified stride.

vDSP_svdivD

Calculates the double-precision element-wise division of a scalar value and a vector, using the specified stride.

### Vector-vector-scalar add-multiply operations

static func multiply&lt;T, U>(addition: (a: T, b: U), Float) -> [Float]

Returns the single-precision element-wise product of the sum of two vectors and a scalar value.

static func multiply&lt;T, U>(addition: (a: T, b: U), Double) -> [Double]

Returns the double-precision element-wise product of the sum of two vectors and a scalar value.

static func multiply&lt;T, U, V>(addition: (a: T, b: U), Float, result: inout V)

Calculates the single-precision element-wise product of the sum of two vectors and a scalar value.

static func multiply&lt;T, U, V>(addition: (a: T, b: U), Double, result: inout V)

Calculates the double-precision element-wise product of the sum of two vectors and a scalar value.

vDSP_vasm

Calculates the single-precision element-wise product of the sum of two vectors and a scalar value, using the specified stride.

vDSP_vasmD

Calculates the double-precision element-wise product of the sum of two vectors and a scalar value, using the specified stride.

### Vector-vector-scalar subtract-multiply operations

static func multiply&lt;T, U>(subtraction: (a: T, b: U), Float) -> [Float]

Returns the single-precision element-wise product of the difference of two vectors and a scalar value.

static func multiply&lt;T, U>(subtraction: (a: T, b: U), Double) -> [Double]

Returns the double-precision element-wise product of the difference of two vectors and a scalar value.

static func multiply&lt;T, U, V>(subtraction: (a: T, b: U), Float, result: inout V)

Calculates the single-precision element-wise product of the difference of two vectors and a scalar value.

static func multiply&lt;T, U, V>(subtraction: (a: T, b: U), Double, result: inout V)

Calculates the double-precision element-wise product of the difference of two vectors and a scalar value.

vDSP_vsbsm

Calculates the single-precision element-wise product of the difference of two vectors and a scalar value, using the specified stride.

vDSP_vsbsmD

Calculates the double-precision element-wise product of the difference of two vectors and a scalar value, using the specified stride.

### Vector-scalar-vector multiply-subtract operations

static func subtract&lt;T, U>(multiplication: (a: U, b: Float), T) -> [Float]

Calculates the single-precision element-wise difference of the product of a vector and a scalar value, and a vector.

static func subtract&lt;T, U>(multiplication: (a: U, b: Double), T) -> [Double]

Calculates the double-precision element-wise difference of the product of a vector and a scalar value, and a vector.

static func subtract&lt;T, U, V>(multiplication: (a: U, b: Float), T, result: inout V)

Calculates the single-precision element-wise difference of the product of a vector and a scalar value, and a vector.

static func subtract&lt;T, U, V>(multiplication: (a: U, b: Double), T, result: inout V)

Calculates the double-precision element-wise difference of the product of a vector and a scalar value, and a vector.

vDSP_vsmsb

Calculates the single-precision element-wise difference of the product of a vector and a scalar value, and a vector, using the specified stride.

vDSP_vsmsbD

Calculates the double-precision element-wise difference of the product of a vector and a scalar value, and a vector, using the specified stride.

### Vector-vector-scalar multiply-add operations

static func add&lt;T, U>(multiplication: (a: T, b: U), Float) -> [Float]

Returns the single-precision element-wise sum of the product of two vectors, and a scalar value.

static func add&lt;T, U>(multiplication: (a: T, b: U), Double) -> [Double]

Returns the double-precision element-wise sum of the product of two vectors, and a scalar value.

static func add&lt;T, U, V>(multiplication: (a: T, b: U), Float, result: inout V)

Calculates the single-precision element-wise sum of the product of two vectors, and a scalar value.

static func add&lt;T, U, V>(multiplication: (a: T, b: U), Double, result: inout V)

Calculates the double-precision element-wise sum of the product of two vectors, and a scalar value.

vDSP_vmsa

Calculates the single-precision element-wise sum of the product of two vectors, and a scalar value, using the specified stride.

vDSP_vmsaD

Calculates the double-precision element-wise sum of the product of two vectors, and a scalar value, using the specified stride.

### Vector-scalar-vector multiply-add operations

static func add&lt;T, U>(multiplication: (a: T, b: Float), U) -> [Float]

Returns the single-precision element-wise addition of the product of a vector and a scalar value, and a vector.

static func add&lt;T, U>(multiplication: (a: T, b: Double), U) -> [Double]

Returns the double-precision element-wise addition of the product of a vector and a scalar value, and a vector.

static func add&lt;T, U, V>(multiplication: (a: T, b: Float), U, result: inout V)

Calculates the single-precision element-wise addition of the product of a vector and a scalar value, and a vector.

static func add&lt;T, U, V>(multiplication: (a: T, b: Double), U, result: inout V)

Calculates the double-precision element-wise addition of the product of a vector and a scalar value, and a vector.

vDSP_vsma

Calculates the single-precision element-wise addition of the product of a vector and a scalar value, and a vector, using the specified stride.

vDSP_vsmaD

Calculates the double-precision element-wise addition of the product of a vector and a scalar value, and a vector, using the specified stride.

### Vector-scalar-scalar multiply-add operations

static func add&lt;U>(multiplication: (a: U, b: Float), Float) -> [Float]

Returns the single-precision element-wise addition of the product of a vector and a scalar value, and a vector.

static func add&lt;U>(multiplication: (a: U, b: Double), Double) -> [Double]

Returns the double-precision element-wise addition of the product of a vector and a scalar value, and a vector.

static func add&lt;U, V>(multiplication: (a: U, b: Float), Float, result: inout V)

Calculates the single-precision element-wise addition of the product of a vector and a scalar value, and a vector.

static func add&lt;U, V>(multiplication: (a: U, b: Double), Double, result: inout V)

Calculates the double-precision element-wise addition of the product of a vector and a scalar value, and a vector.

vDSP_vsmsa

Calculates the single-precision element-wise addition of the product of a vector and a scalar value, and a scalar value, using the specified stride.

vDSP_vsmsaD

Calculates the double-precision element-wise addition of the product of a vector and a scalar value, and a scalar value, using the specified stride.

### Vector-scalar-vector-scalar multiply-multiply-add operations

static func add&lt;T, U>(multiplication: (a: T, b: Float), multiplication: (c: U, d: Float)) -> [Float]

Returns the single-precision element-wise addition of two vector-scalar products.

static func add&lt;T, U>(multiplication: (a: T, b: Double), multiplication: (c: U, d: Double)) -> [Double]

Returns the double-precision element-wise addition of two vector-scalar products.

static func add&lt;T, U, V>(multiplication: (a: T, b: Float), multiplication: (c: U, d: Float), result: inout V)

Calculates the single-precision element-wise addition of two vector-scalar products.

static func add&lt;T, U, V>(multiplication: (a: T, b: Double), multiplication: (c: U, d: Double), result: inout V)

Calculates the double-precision element-wise addition of two vector-scalar products.

vDSP_vsmsma

Calculates the single-precision element-wise addition of two vector-scalar products, using the specified stride.

vDSP_vsmsmaD

Calculates the double-precision element-wise addition of two vector-scalar products, using the specified stride.

