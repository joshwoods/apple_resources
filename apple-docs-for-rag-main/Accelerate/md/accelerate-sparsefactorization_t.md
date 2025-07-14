

- Accelerate
-  SparseFactorization_t 

Structure

# SparseFactorization_t

Constants that define the factorization type.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct SparseFactorization_t
```

## Topics

### Factorization Types for Symmetric Coefficient Matrices

var SparseFactorizationCholesky: SparseFactorization_t

A constant that represents Cholesky (*LLᵀ*) factorization.

var SparseFactorizationLDLT: SparseFactorization_t

A constant that represents the default *LDLᵀ* factorization.

var SparseFactorizationLDLTUnpivoted: SparseFactorization_t

A constant that represents Cholesky-like *LDLᵀ* factorization with only one-by-one pivots and no pivoting.

var SparseFactorizationLDLTSBK: SparseFactorization_t

A constant that represents *LDLᵀ* factorization with Supernode-Bunch-Kaufman and static pivoting.

var SparseFactorizationLDLTTPP: SparseFactorization_t

A constant that represents *LDLᵀ* factorization with full-threshold partial pivoting.

### Factorization Types for Overdetermined and Underdetermined Systems

var SparseFactorizationQR: SparseFactorization_t

A constant that represents QR factorization.

var SparseFactorizationCholeskyAtA: SparseFactorization_t

A constant that represents *QR* factorization without storing *Q*.

### Raw Values

init(UInt8)

init(rawValue: UInt8)

var rawValue: UInt8

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Structures that Specify Factorization Type and Factorization Options

struct SparseSymbolicFactorOptions

A structure that contains options that affect the symbolic stage of a sparse factorization.

struct SparseNumericFactorOptions

A structure that contains options that affect the numerical stage of a sparse factorization.

