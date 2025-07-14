

- Accelerate
- SparseOpaquePreconditioner_Float
-  type 

Instance Property

# type

The preconditioner type.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var type: SparsePreconditioner_t
```

## See Also

### Inspecting Preconditioner Properties

var apply: (UnsafeMutableRawPointer, CBLAS_TRANSPOSE, DenseMatrix_Float, DenseMatrix_Float) -> Void

A function that calculates *Y = PX*, where *P* is the preconditioner.

var mem: UnsafeMutableRawPointer

The unaltered memory pointer that passes as the first parameter of the apply function.

