

- Accelerate
- SparseOpaquePreconditioner_Float
-  init(type:mem:apply:) 

Initializer

# init(type:mem:apply:)

Creates a new single-precision preconditioner.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    type: SparsePreconditioner_t,
    mem: UnsafeMutableRawPointer,
    apply: (UnsafeMutableRawPointer, CBLAS_TRANSPOSE, DenseMatrix_Float, DenseMatrix_Float) -> Void
)
```

## Parameters 

`type`  

The preconditioner type.

`mem`  

The unaltered memory pointer that passes as the first parameter of the `apply` function.

`apply`  

A function that calculates *Y = PX*, where *P* is the preconditioner.

