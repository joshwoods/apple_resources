

- Accelerate
- SparseOpaqueFactorization_Double
-  status 

Instance Property

# status

The status of the factorization object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var status: SparseStatus_t
```

## See Also

### Instance Properties

var attributes: SparseAttributes_t

The attributes of a factorization object.

var numericFactorization: UnsafeMutableRawPointer?

The pointer to a private internal representation of a numeric factor.

var solveWorkspaceRequiredPerRHS: Int

The required size of the per-right-hand-side workspace for a call to a sparse solve function.

var solveWorkspaceRequiredStatic: Int

The required size of the static workspace for a call to a sparse solve function.

var symbolicFactorization: SparseOpaqueSymbolicFactorization

The symbolic factorization that this numeric factorization depends on.

var userFactorStorage: Bool

A Boolean value that indicates whether user-provided storage backs this object.

