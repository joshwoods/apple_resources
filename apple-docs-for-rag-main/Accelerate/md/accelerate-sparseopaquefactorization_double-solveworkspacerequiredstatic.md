

- Accelerate
- SparseOpaqueFactorization_Double
-  solveWorkspaceRequiredStatic 

Instance Property

# solveWorkspaceRequiredStatic

The required size of the static workspace for a call to a sparse solve function.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var solveWorkspaceRequiredStatic: Int
```

## Discussion

The required size of workspace in bytes for a call to a sparse solve function is solveWorkspaceRequiredStatic `+ nrhs *` solveWorkspaceRequiredPerRHS where `nrhs` is the number of right-hand-side vectors.

## See Also

### Instance Properties

var attributes: SparseAttributes_t

The attributes of a factorization object.

var numericFactorization: UnsafeMutableRawPointer?

The pointer to a private internal representation of a numeric factor.

var solveWorkspaceRequiredPerRHS: Int

The required size of the per-right-hand-side workspace for a call to a sparse solve function.

var status: SparseStatus_t

The status of the factorization object.

var symbolicFactorization: SparseOpaqueSymbolicFactorization

The symbolic factorization that this numeric factorization depends on.

var userFactorStorage: Bool

A Boolean value that indicates whether user-provided storage backs this object.

