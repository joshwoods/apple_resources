

- Accelerate
-  SparseStatus_t 

Structure

# SparseStatus_t

Constants that describe the status of a factorization.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct SparseStatus_t
```

## Topics

### Constants

init(Int32)

init(rawValue: Int32)

var rawValue: Int32

var SparseStatusOK: SparseStatus_t

The factorization was successful.

var SparseFactorizationFailed: SparseStatus_t

The factorization failed due to a numerical issue.

var SparseMatrixIsSingular: SparseStatus_t

The factorization aborted because the matrix is singular.

var SparseInternalError: SparseStatus_t

The factorization encountered an internal error, such as failing to allocate memory.

var SparseParameterError: SparseStatus_t

An error in a user-supplied parameter.

var SparseStatusReleased: SparseStatus_t

The system freed the factorization object.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Instance Properties

var status: SparseStatus_t

The status of the factorization.

var type: SparseFactorization_t

The factorization type.

var factorization: UnsafeMutableRawPointer?

A pointer to a private internal representation of the symbolic factor.

struct SparseFactorization_t

Constants that define the factorization type.

