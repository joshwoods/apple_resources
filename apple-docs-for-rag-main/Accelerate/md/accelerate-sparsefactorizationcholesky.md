

- Accelerate
-  SparseFactorizationCholesky 

Global Variable

# SparseFactorizationCholesky

A constant that represents Cholesky (*LLᵀ*) factorization.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var SparseFactorizationCholesky: SparseFactorization_t { get }
```

## Discussion

SparseFactorizationCholesky provides a sparse counterpart to the dense Cholesky routines `spotrf()` and `dpotrf()` from LAPACK.

## See Also

### Factorization Types for Symmetric Coefficient Matrices

var SparseFactorizationLDLT: SparseFactorization_t

A constant that represents the default *LDLᵀ* factorization.

var SparseFactorizationLDLTUnpivoted: SparseFactorization_t

A constant that represents Cholesky-like *LDLᵀ* factorization with only one-by-one pivots and no pivoting.

var SparseFactorizationLDLTSBK: SparseFactorization_t

A constant that represents *LDLᵀ* factorization with Supernode-Bunch-Kaufman and static pivoting.

var SparseFactorizationLDLTTPP: SparseFactorization_t

A constant that represents *LDLᵀ* factorization with full-threshold partial pivoting.

