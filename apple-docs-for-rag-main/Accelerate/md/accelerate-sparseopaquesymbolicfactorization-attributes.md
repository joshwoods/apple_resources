

- Accelerate
- SparseOpaqueSymbolicFactorization
-  attributes 

Instance Property

# attributes

The attributes of the factorization.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var attributes: SparseAttributes_t
```

## See Also

### Inspecting a Factorization’s Structure

struct SparseAttributes_t

A structure that represents the attributes of a matrix.

var blockSize: UInt8

The block size.

var columnCount: Int32

The number of columns.

var rowCount: Int32

The number of rows.

var workspaceSize_Double: Int

Size, in bytes, of workspace required to perform numerical factorization in doubles.

var workspaceSize_Float: Int

Size, in bytes, of workspace required to perform numerical factorization in floats.

var factorSize_Double: Int

Minimum size, in bytes, required to store numerical factors in doubles.

var factorSize_Float: Int

Minimum size, in bytes, required to store numerical factors in float.

