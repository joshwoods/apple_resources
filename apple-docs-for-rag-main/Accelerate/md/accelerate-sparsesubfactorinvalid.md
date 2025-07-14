

- Accelerate
-  SparseSubfactorInvalid 

Global Variable

# SparseSubfactorInvalid

An invalid subfactor that indicates the requested type is incompatible with the supplied factorization or the system has destroyed it.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var SparseSubfactorInvalid: SparseSubfactor_t { get }
```

## See Also

### Constants

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

