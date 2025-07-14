

- Accelerate
- vDSP
-  Complex basic arithmetic 

API Collection

# Complex basic arithmetic

Perform elementwise operations on vectors of complex values.

## Topics

### Binary Addition Operations

vDSP_zvadd

Adds two single-precision complex vectors.

vDSP_zvaddD

Adds two double-precision complex vectors.

### Binary Subtraction Operations

vDSP_zvsub

Subtracts two single-precision complex vectors.

vDSP_zvsubD

Subtracts two double-precision complex vectors.

### Binary Conjugate-Multiply Operations

vDSP_zvcmul

Multiplies a single-precision complex vector by the conjugate of another single-precision complex vector.

vDSP_zvcmulD

Multiplies a double-precision complex vector by the conjugate of another double-precision complex vector.

### Binary Optional Conjugate-Multiply Operations

vDSP_zvmul

Multiplies a single-precision complex vector by the optionally conjugate of another single-precision complex vector.

vDSP_zvmulD

Multiplies a double-precision complex vector by the optionally conjugate of another double-precision complex vector.

### Binary Division Operations

vDSP_zvdiv

Divides two complex single-precision vectors.

vDSP_zvdivD

Divides two complex double-precision vectors.

### Binary Transfer Operations

vDSP_ztrans

Divides a complex single-precision vector by a real single-precision vector.

vDSP_ztransD

Divides a complex double-precision vector by a real double-precision vector.

### Binary (Complex-Real) Addition Operations

vDSP_zrvadd

Adds a single-precision complex vector to a single-precision real vector.

vDSP_zrvaddD

Adds a double-precision complex vector to a double-precision real vector.

### Binary (Complex-Real) Subtraction Operations

vDSP_zrvsub

Subtracts a single-precision real vector from a single-precision complex vector.

vDSP_zrvsubD

Subtracts a double-precision real vector from a double-precision complex vector.

### Binary (Complex-Real) Multiplication Operations

vDSP_zrvmul

Multiplies a single-precision complex vector by a single-precision real vector.

vDSP_zrvmulD

Multiplies a double-precision complex vector by a double-precision real vector.

### Binary (Complex-Real) Division Operations

vDSP_zrvdiv

Divides a single-precision complex vector by a single-precision real vector.

vDSP_zrvdivD

Divides a double-precision complex vector by a double-precision real vector.

### Ternary Multiply-Add Operations

vDSP_zvma

Adds a single-precision complex vector to the product of two single-precision complex vectors.

vDSP_zvmaD

Adds a double-precision complex vector to the product of two double-precision complex vectors.

### Ternary Conjugate-Multiply-Add

vDSP_zvcma

Adds a single-precision complex vector to the product of a single-precision complex vector and the conjugate of another complex single-precision vector.

vDSP_zvcmaD

Adds a double-precision complex vector to the product of a double-precision complex vector and the conjugate of another complex double-precision vector.

### Quinary Multiply-Multiply-Add-Add

vDSP_zvmmaa

Adds a single-precision complex vector to the sum of the product of two single-precision complex vectors and a second product of two single-precision complex vectors.

vDSP_zvmmaaD

Adds a double-precision complex vector to the sum of the product of two double-precision complex vectors and a second product of two double-precision complex vectors.

## See Also

### Vector-vector arithmetic

Vector-vector real arithmetic functions

Perform element-wise operations on vectors of real values.

Integer arithmetic

Perform elementwise operations on vectors of integer values.

Linear averaging functions

Calculate the element-wise linear average of two vectors.

Polynomial evaluation

Evaluate polynomials using coefficients and independent variables that you supply.

