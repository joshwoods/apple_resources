

- Accelerate
-  SparseInternalError 

Global Variable

# SparseInternalError

The factorization encountered an internal error, such as failing to allocate memory.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var SparseInternalError: SparseStatus_t { get }
```

## See Also

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

var SparseParameterError: SparseStatus_t

An error in a user-supplied parameter.

var SparseStatusReleased: SparseStatus_t

The system freed the factorization object.

