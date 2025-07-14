

- Accelerate
-  SparseStatusReleased 

Global Variable

# SparseStatusReleased

The system freed the factorization object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var SparseStatusReleased: SparseStatus_t { get }
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

var SparseInternalError: SparseStatus_t

The factorization encountered an internal error, such as failing to allocate memory.

var SparseParameterError: SparseStatus_t

An error in a user-supplied parameter.

