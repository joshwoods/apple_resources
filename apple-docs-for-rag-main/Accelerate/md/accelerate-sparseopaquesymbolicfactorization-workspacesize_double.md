

- Accelerate
- SparseOpaqueSymbolicFactorization
-  workspaceSize_Double 

Instance Property

# workspaceSize_Double

Size, in bytes, of workspace required to perform numerical factorization in doubles.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var workspaceSize_Double: Int
```

## See Also

### Inspecting a Factorization’s Structure

var attributes: SparseAttributes_t

The attributes of the factorization.

struct SparseAttributes_t

A structure that represents the attributes of a matrix.

var blockSize: UInt8

The block size.

var columnCount: Int32

The number of columns.

var rowCount: Int32

The number of rows.

var workspaceSize_Float: Int

Size, in bytes, of workspace required to perform numerical factorization in floats.

var factorSize_Double: Int

Minimum size, in bytes, required to store numerical factors in doubles.

var factorSize_Float: Int

Minimum size, in bytes, required to store numerical factors in float.

