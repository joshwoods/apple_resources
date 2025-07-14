

- Accelerate
- SparseMatrix_Double
-  data 

Instance Property

# data

The array of contiguous values in the nonzero blocks of the matrix.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var data: UnsafeMutablePointer
```

## Discussion

The matrix stores each block in column-major order. The number of elements in data must be equal to blockSize x blockSize x the number of nonzero blocks in the matrix.

## See Also

### Inspecting a Matrix’s Structure and Data

var structure: SparseMatrixStructure

The sparsity structure of the matrix.

