

- Accelerate
- SparseOpaqueFactorization_Float
-  userFactorStorage 

Instance Property

# userFactorStorage

A Boolean value that indicates whether user-provided storage backs this object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var userFactorStorage: Bool
```

## Discussion

If true, the user must free factor storage after all references finish (though SparseCleanup(_:)) still frees any additional allocated storage due to pivoting).

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

var status: SparseStatus_t

The status of the factorization object.

var symbolicFactorization: SparseOpaqueSymbolicFactorization

The symbolic factorization that this numeric factorization depends on.

