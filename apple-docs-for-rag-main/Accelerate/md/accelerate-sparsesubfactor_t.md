

- Accelerate
-  SparseSubfactor_t 

Structure

# SparseSubfactor_t

Constants that define the subfactor of a factorization.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct SparseSubfactor_t
```

## Topics

### Constants

var SparseSubfactorInvalid: SparseSubfactor_t

An invalid subfactor that indicates the requested type is incompatible with the supplied factorization or the system has destroyed it.

var SparseSubfactorP: SparseSubfactor_t

A permutation subfactor that’s valid for all factorization types.

var SparseSubfactorS: SparseSubfactor_t

A diagonal scaling subfactor that’s valid for Cholesky and *LDLᵀ* only.

var SparseSubfactorL: SparseSubfactor_t

An *L* factor subfactor that’s valid for Cholesky and *LDLᵀ* only.

var SparseSubfactorD: SparseSubfactor_t

A *D* factor subfactor that’s valid for *LDLᵀ*only.

var SparseSubfactorPLPS: SparseSubfactor_t

A half-solve subfactor that’s valid for Cholesky and *LDLᵀ* only.

var SparseSubfactorQ: SparseSubfactor_t

A *Q* factor subfactor that’s valid for QR only.

var SparseSubfactorR: SparseSubfactor_t

An *R* factor subfactor that’s valid for QR and Cholesky *AᵀA* only.

var SparseSubfactorRP: SparseSubfactor_t

A half-solve subfactor that’s valid for QR and Cholesky *AᵀA* only.

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

### Subfactor Extraction

func SparseCreateSubfactor(SparseSubfactor_t, SparseOpaqueFactorization_Double) -> SparseOpaqueSubfactor_Double

Returns an opaque object that represents a subfactor of a factorization of a matrix of double-precision values.

struct SparseOpaqueFactorization_Double

A structure that represents the factorization of a matrix of double-precision, floating-point values.

func SparseCreateSubfactor(SparseSubfactor_t, SparseOpaqueFactorization_Float) -> SparseOpaqueSubfactor_Float

Returns an opaque object that represents a subfactor of a factorization of a matrix of single-precision values.

struct SparseOpaqueFactorization_Float

A structure that represents the factorization of a matrix of single-precision, floating-point values.

