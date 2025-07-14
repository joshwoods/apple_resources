

- Accelerate
- SparseOpaquePreconditioner_Double
-  mem 

Instance Property

# mem

The unaltered memory pointer that passes as the first parameter of the apply function.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var mem: UnsafeMutableRawPointer
```

## See Also

### Inspecting Preconditioner Properties

var apply: (UnsafeMutableRawPointer, CBLAS_TRANSPOSE, DenseMatrix_Double, DenseMatrix_Double) -> Void

A function that calculates *Y = PX*, where *P* is the preconditioner.

var type: SparsePreconditioner_t

The preconditioner type.

