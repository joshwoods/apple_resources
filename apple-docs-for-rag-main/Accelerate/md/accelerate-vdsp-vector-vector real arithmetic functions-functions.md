

- Accelerate
- vDSP
-  Vector-vector real arithmetic functions 

API Collection

# Vector-vector real arithmetic functions

Perform element-wise operations on vectors of real values.

## Overview

The vDSP library provides a suite of general-purpose, high-performance arithmetic functions that are alternatives to `for` loops and `map` when you apply operations on collections of floating-point values.

See Using vDSP for vector-based arithmetic for a summary of available operations.

## Topics

### Binary addition operations

static func add&lt;T, U>(T, U) -> [Float]

Returns the single-precision element-wise sum of two vectors.

static func add&lt;T, U>(T, U) -> [Double]

Returns the double-precision element-wise sum of two vectors.

static func add&lt;T, U, V>(T, U, result: inout V)

Calculates the single-precision element-wise sum of two vectors.

static func add&lt;T, U, V>(T, U, result: inout V)

Calculates the double-precision element-wise sum of two vectors.

vDSP_vadd

Calculates the single-precision element-wise sum of two vectors, using the specified stride.

vDSP_vaddD

Calculates the double-precision element-wise sum of two vectors, using the specified stride.

### Binary subtraction operations

static func subtract&lt;T, U>(U, T) -> [Float]

Returns the single-precision element-wise subtraction of two vectors.

static func subtract&lt;T, U>(U, T) -> [Double]

Returns the double-precision element-wise subtraction of two vectors.

static func subtract&lt;T, U, V>(U, T, result: inout V)

Calculates the single-precision element-wise subtraction of two vectors.

static func subtract&lt;T, U, V>(U, T, result: inout V)

Calculates the double-precision element-wise subtraction of two vectors.

vDSP_vsub

Calculates the single-precision element-wise subtraction of two vectors, using the specified stride.

vDSP_vsubD

Calculates the double-precision element-wise subtraction of two vectors, using the specified stride.

### Binary multiplication operations

static func multiply&lt;T, U>(T, U) -> [Float]

Returns the single-precision element-wise product of two vectors.

static func multiply&lt;T, U>(T, U) -> [Double]

Returns the double-precision element-wise product of two vectors.

static func multiply&lt;T, U, V>(T, U, result: inout V)

Calculates the single-precision element-wise product of two vectors.

static func multiply&lt;T, U, V>(T, U, result: inout V)

Calculates the double-precision element-wise product of two vectors.

vDSP_vmul

Calculates the single-precision element-wise product of two vectors, using the specified stride.

vDSP_vmulD

Calculates the double-precision element-wise product of two vectors, using the specified stride.

### Binary division operations

static func divide&lt;T, U>(T, U) -> [Float]

Returns the single-precision element-wise division of two vectors.

static func divide&lt;T, U>(T, U) -> [Double]

Returns the double-precision element-wise division of two vectors.

static func divide&lt;T, U, V>(T, U, result: inout V)

Calculates the single-precision element-wise division of two vectors.

static func divide&lt;T, U, V>(T, U, result: inout V)

Calculates the double-precision element-wise division of two vectors.

vDSP_vdiv

Calculates the single-precision element-wise division of two vectors, using the specified stride.

vDSP_vdivD

Calculates the double-precision element-wise division of two vectors, using the specified stride.

### Binary addition and subtraction operations

static func addSubtract&lt;S, T, U, V>(S, T, addResult: inout U, subtractResult: inout V)

Calculates the single-precision element-wise sum and subtraction of two vectors.

static func addSubtract&lt;S, T, U, V>(S, T, addResult: inout U, subtractResult: inout V)

Calculates the double-precision element-wise sum and subtraction of two vectors.

vDSP_vaddsub

Calculates the single-precision element-wise sum and subtraction of two vectors, using the specified stride.

vDSP_vaddsubD

Calculates the double-precision element-wise sum and subtraction of two vectors, using the specified stride.

### Ternary add-multiply operations

static func multiply&lt;S, T, U>(addition: (a: S, b: T), U) -> [Float]

Returns the single-precision element-wise product of a vector and the sum of two vectors.

static func multiply&lt;S, T, U>(addition: (a: S, b: T), U) -> [Double]

Returns the double-precision element-wise product of a vector and the sum of two vectors.

static func multiply&lt;S, T, U, V>(addition: (a: S, b: T), U, result: inout V)

Calculates the single-precision element-wise product of a vector and the sum of two vectors.

static func multiply&lt;S, T, U, V>(addition: (a: S, b: T), U, result: inout V)

Calculates the double-precision element-wise product of a vector and the sum of two vectors.

vDSP_vam

Calculates the single-precision element-wise product of a vector and the sum of two vectors, using the specified stride.

vDSP_vamD

Calculates the double-precision element-wise product of a vector and the sum of two vectors, using the specified stride.

### Ternary multiply-add operations

static func add&lt;S, T, U>(multiplication: (a: S, b: T), U) -> [Float]

Returns the single-precision element-wise sum of a vector and the product of two vectors.

static func add&lt;S, T, U>(multiplication: (a: S, b: T), U) -> [Double]

Returns the double-precision element-wise sum of a vector and the product of two vectors.

static func add&lt;S, T, U, V>(multiplication: (a: S, b: T), U, result: inout V)

Calculates the single-precision element-wise sum of a vector and the product of two vectors.

static func add&lt;S, T, U, V>(multiplication: (a: S, b: T), U, result: inout V)

Calculates the double-precision element-wise sum of a vector and the product of two vectors.

vDSP_vma

Calculates the single-precision element-wise sum of a vector and the product of two vectors, using the specified stride.

vDSP_vmaD

Calculates the double-precision element-wise sum of a vector and the product of two vectors, using the specified stride.

### Ternary multiply-subtract operations

static func subtract&lt;S, T, U>(multiplication: (a: T, b: U), S) -> [Float]

Returns the single-precision element-wise difference of a vector and the product of two vectors.

static func subtract&lt;S, T, U>(multiplication: (a: T, b: U), S) -> [Double]

Returns the double-precision element-wise difference of a vector and the product of two vectors.

static func subtract&lt;S, T, U, V>(multiplication: (a: T, b: U), S, result: inout V)

Calculates the single-precision element-wise difference of a vector and the product of two vectors.

static func subtract&lt;S, T, U, V>(multiplication: (a: T, b: U), S, result: inout V)

Calculates the double-precision element-wise difference of a vector and the product of two vectors.

vDSP_vmsb

Calculates the single-precision element-wise difference of a vector and the product of two vectors, using the specified stride.

vDSP_vmsbD

Calculates the double-precision element-wise difference of a vector and the product of two vectors, using the specified stride.

### Ternary subtract-multiply operations

static func multiply&lt;S, T, U>(subtraction: (a: S, b: T), U) -> [Float]

Returns the single-precision element-wise product of a vector and the differences of two vectors.

static func multiply&lt;S, T, U>(subtraction: (a: S, b: T), U) -> [Double]

Returns the double-precision element-wise product of a vector and the differences of two vectors.

static func multiply&lt;S, T, U, V>(subtraction: (a: S, b: T), U, result: inout V)

Calculates the single-precision element-wise product of a vector and the differences of two vectors.

static func multiply&lt;S, T, U, V>(subtraction: (a: S, b: T), U, result: inout V)

Calculates the double-precision element-wise product of a vector and the differences of two vectors.

vDSP_vsbm

Calculates the single-precision element-wise product of a vector and the differences of two vectors, using the specified stride.

vDSP_vsbmD

Calculates the double-precision element-wise product of a vector and the differences of two vectors, using the specified stride.

### Quaternary multiply-multiply-add operations

vDSP_vmma

Calculates the single-precision element-wise sum of the products of two pairs of vectors, using the specified stride.

vDSP_vmmaD

Calculates the double-precision element-wise sum of the products of two pairs of vectors, using the specified stride.

### Quaternary multiply-multiply-subtract operations

static func subtract&lt;R, S, T, U>(multiplication: (a: T, b: U), multiplication: (c: R, d: S)) -> [Float]

Returns the single-precision element-wise difference of the products of two pairs of vectors.

static func subtract&lt;R, S, T, U>(multiplication: (a: T, b: U), multiplication: (c: R, d: S)) -> [Double]

Returns the double-precision element-wise difference of the products of two pairs of vectors.

static func subtract&lt;R, S, T, U, V>(multiplication: (a: T, b: U), multiplication: (c: R, d: S), result: inout V)

Calculates the single-precision element-wise difference of the products of two pairs of vectors.

static func subtract&lt;R, S, T, U, V>(multiplication: (a: T, b: U), multiplication: (c: R, d: S), result: inout V)

Calculates the double-precision element-wise difference of the products of two pairs of vectors.

vDSP_vmmsb

Calculates the single-precision element-wise difference of the products of two pairs of vectors, using the specified stride.

vDSP_vmmsbD

Calculates the double-precision element-wise difference of the products of two pairs of vectors, using the specified stride.

### Quaternary add-add-multiply operations

static func multiply&lt;S, T, U>(addition: (a: S, b: T), addition: (c: U, d: U)) -> [Float]

Returns the single-precision element-wise product of the sums of two pairs of vectors.

static func multiply&lt;S, T, U>(addition: (a: S, b: T), addition: (c: U, d: U)) -> [Double]

Returns the double-precision element-wise product of the sums of two pairs of vectors.

static func multiply&lt;S, T, U, V>(addition: (a: S, b: T), addition: (c: U, d: U), result: inout V)

Calculates the single-precision element-wise product of the sums of two pairs of vectors.

static func multiply&lt;S, T, U, V>(addition: (a: S, b: T), addition: (c: U, d: U), result: inout V)

Calculates the double-precision element-wise product of the sums of two pairs of vectors.

vDSP_vaam

Calculates the single-precision element-wise product of the sums of two pairs of vectors, using the specified stride.

vDSP_vaamD

Calculates the double-precision element-wise product of the sums of two pairs of vectors, using the specified stride.

### Quaternary subtract-subtract-multiply operations

static func multiply&lt;R, S, T, U>(subtraction: (a: R, b: S), subtraction: (c: T, d: U)) -> [Float]

Returns the single-precision element-wise product of the differences of two pairs of vectors.

static func multiply&lt;R, S, T, U>(subtraction: (a: R, b: S), subtraction: (c: T, d: U)) -> [Double]

Returns the double-precision element-wise product of the differences of two pairs of vectors.

static func multiply&lt;R, S, T, U, V>(subtraction: (a: R, b: S), subtraction: (c: T, d: U), result: inout V)

Calculates the single-precision element-wise product of the differences of two pairs of vectors.

static func multiply&lt;R, S, T, U, V>(subtraction: (a: R, b: S), subtraction: (c: T, d: U), result: inout V)

Calculates the double-precision element-wise product of the differences of two pairs of vectors.

vDSP_vsbsbm

Calculates the single-precision element-wise product of the differences of two pairs of vectors, using the specified stride.

vDSP_vsbsbmD

Calculates the double-precision element-wise product of the differences of two pairs of vectors, using the specified stride.

### Quaternary add-subtract-multiply operations

static func multiply&lt;R, S, T, U>(addition: (a: R, b: S), subtraction: (c: T, d: U)) -> [Float]

Returns the single-precision element-wise product of the sum of two vectors and the difference of two vectors.

static func multiply&lt;R, S, T, U>(addition: (a: R, b: S), subtraction: (c: T, d: U)) -> [Double]

Returns the double-precision element-wise product of the sum of two vectors and the difference of two vectors.

static func multiply&lt;R, S, T, U, V>(addition: (a: R, b: S), subtraction: (c: T, d: U), result: inout V)

Calculates the double-precision element-wise product of the sum of two vectors and the difference of two vectors.

static func multiply&lt;R, S, T, U, V>(addition: (a: R, b: S), subtraction: (c: T, d: U), result: inout V)

Calculates the double-precision element-wise product of the sum of two vectors and the difference of two vectors.

vDSP_vasbm

Calculates the double-precision element-wise product of the sum of two vectors and the difference of two vectors, using the specified stride.

vDSP_vasbmD

Calculates the double-precision element-wise product of the sum of two vectors and the difference of two vectors, using the specified stride.

## See Also

### Vector-vector arithmetic

Complex basic arithmetic

Perform elementwise operations on vectors of complex values.

Integer arithmetic

Perform elementwise operations on vectors of integer values.

Linear averaging functions

Calculate the element-wise linear average of two vectors.

Polynomial evaluation

Evaluate polynomials using coefficients and independent variables that you supply.

