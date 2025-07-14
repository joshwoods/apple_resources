

- Accelerate
- SparseOpaqueSubfactor_Double
-  contents 

Instance Property

# contents

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var contents: SparseSubfactor_t
```

## Discussion

Invalid subfactor (requested type not compatible with supplied factorization or already destroyed).

Permutation subfactor, valid for all factorization types.

Diagonal scaling subfactor, valid for Cholesky and LDL^T only.

L factor subfactor, valid for Cholesky and LDL^T only.

D factor subfactor, valid for LDL^T only.

Half-solve subfactor, valid for Cholesky and LDL^T only. Corresponds to PLP’ on forward (non-transpose) solve, and corresponds to PLDP’ on backward (transpose) solve (D=I for Chokesky).

Q factor subfactor, valid for QR only.

R factor subfactor, valid for QR and CholeskyAtA only.

Half-solve subfactor, valid for QR and CholeskyAtA only.

