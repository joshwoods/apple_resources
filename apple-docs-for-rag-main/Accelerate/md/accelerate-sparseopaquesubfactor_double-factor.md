

- Accelerate
- SparseOpaqueSubfactor_Double
-  factor 

Instance Property

# factor

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var factor: SparseOpaqueFactorization_Double
```

## Discussion

Use the `SparseCleanup` function to free resources held by these objects.

The object can be in one of the following states:

1.  Something went wrong with symbolic factorization, nothing is valid.

    - indicated by .symbolicFactorization.status \= 0 && .status \= 0 && .status \= 0

Indicates status of factorization object.

Flags associated with this factorization object. In particular, transpose field indicates whether object is considered to be factorization of A or A^T.

Symbolic Factorization upon which this Numeric Factorization depends.

Flag that indicates if user provided storage backing this object. If true, then factor storage must be freed by the user once all references are finished with (though any additional storage allocated due to pivoting will still be freed by SparseCleanup()).

Pointer to private internal representation of numeric factor.

The required size of workspace, in bytes) for a call to SparseSolve is solveWorkspaceRequiredStatic + nrhs \* solveWorkspaceRequiredPerRHS where nrhs is the number of right-hand side vectors.

The required size of workspace, in bytes) for a call to SparseSolve is solveWorkspaceRequiredStatic + nrhs \* solveWorkspaceRequiredPerRHS where nrhs is the number of right-hand side vectors.

