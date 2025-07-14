

- Accelerate
- DenseMatrix_Float
-  init(rowCount:columnCount:columnStride:attributes:data:) 

Initializer

# init(rowCount:columnCount:columnStride:attributes:data:)

Creates a new matrix of single-precision values.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    rowCount: Int32,
    columnCount: Int32,
    columnStride: Int32,
    attributes: SparseAttributes_t,
    data: UnsafeMutablePointer
)
```

## Parameters 

`rowCount`  

The number of rows in the matrix.

`columnCount`  

The number of columns in the matrix.

`columnStride`  

The column stride of the matrix.

`attributes`  

The attributes of the matrix, such as whether it’s symmetrical or triangular.

`data`  

The array of single-precision, floating-point values in column-major order.

