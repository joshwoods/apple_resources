

- Core Image
- CIDataMatrixCodeDescriptor
-  init(payload:rowCount:columnCount:eccVersion:) 

Initializer

# init(payload:rowCount:columnCount:eccVersion:)

Initializes a descriptor that can be used as input to the `CIBarcodeGenerator` filter.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
init?(
    payload errorCorrectedPayload: Data,
    rowCount: Int,
    columnCount: Int,
    eccVersion: CIDataMatrixCodeDescriptor.ECCVersion
)
```

## Parameters 

`errorCorrectedPayload`  

The data to encode in the Data Matrix code.

`rowCount`  

The number of rows in the matrix.

`columnCount`  

The number of columns in the matrix.

`eccVersion`  

The code's ECC version. Valid values are 000, 050, 080, 100, 140, and 200.

Any symbol with an even number of rows and columns will be ECC 200.

## Return Value

A Data Matrix code descriptor encoding the specified payload in the specified row and column count under the specified ECC version.

## Discussion

The `CIBarcodeGenerator` filter can recreate a Data Matrix code given the descriptor created using this method.

