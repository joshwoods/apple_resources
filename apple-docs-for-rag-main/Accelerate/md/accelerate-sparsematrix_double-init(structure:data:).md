

- Accelerate
- SparseMatrix_Double
-  init(structure:data:) 

Initializer

# init(structure:data:)

Creates a sparse matrix with the specified structure that contains double-precision values.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    structure: SparseMatrixStructure,
    data: UnsafeMutablePointer
)
```

## Parameters 

`structure`  

The sparsity structure of the matrix.

`data`  

The array of contiguous values in the nonzero blocks of the matrix. The matrix stores each block in column-major order. The number of elements in data must be equal to blockSize x blockSize x the number of nonzero blocks in the matrix.

