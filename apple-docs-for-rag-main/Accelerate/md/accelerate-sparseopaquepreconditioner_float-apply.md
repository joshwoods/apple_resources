

- Accelerate
- SparseOpaquePreconditioner_Float
-  apply 

Instance Property

# apply

A function that calculates *Y = PX*, where *P* is the preconditioner.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var apply: (UnsafeMutableRawPointer, CBLAS_TRANSPOSE, DenseMatrix_Float, DenseMatrix_Float) -> Void
```

## Discussion

The function has some approximation to *A⁻¹*.

## See Also

### Inspecting Preconditioner Properties

var mem: UnsafeMutableRawPointer

The unaltered memory pointer that passes as the first parameter of the apply function.

var type: SparsePreconditioner_t

The preconditioner type.

