

- Accelerate
-  SparseFactorizationLDLT 

Global Variable

# SparseFactorizationLDLT

A constant that represents the default *LDLᵀ* factorization.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var SparseFactorizationLDLT: SparseFactorization_t { get }
```

## Discussion

SparseFactorizationLDLT provides a sparse counterpart to the dense *LDL\_\_ᵀ* routines `ssytrf()` and `dsytrf()` from LAPACK.

## See Also

### Factorization Types for Symmetric Coefficient Matrices

var SparseFactorizationCholesky: SparseFactorization_t

A constant that represents Cholesky (*LLᵀ*) factorization.

var SparseFactorizationLDLTUnpivoted: SparseFactorization_t

A constant that represents Cholesky-like *LDLᵀ* factorization with only one-by-one pivots and no pivoting.

var SparseFactorizationLDLTSBK: SparseFactorization_t

A constant that represents *LDLᵀ* factorization with Supernode-Bunch-Kaufman and static pivoting.

var SparseFactorizationLDLTTPP: SparseFactorization_t

A constant that represents *LDLᵀ* factorization with full-threshold partial pivoting.

