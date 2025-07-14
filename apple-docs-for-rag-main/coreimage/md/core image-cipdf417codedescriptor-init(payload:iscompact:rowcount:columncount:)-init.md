

- Core Image
- CIPDF417CodeDescriptor
-  init(payload:isCompact:rowCount:columnCount:) 

Initializer

# init(payload:isCompact:rowCount:columnCount:)

Initializes a descriptor that can be used as input to the `CIBarcodeGenerator` filter.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
init?(
    payload errorCorrectedPayload: Data,
    isCompact: Bool,
    rowCount: Int,
    columnCount: Int
)
```

## Parameters 

`errorCorrectedPayload`  

The data to encode in the PDF417 code.

`isCompact`  

A Boolean specifying whether or not the code is compact.

`rowCount`  

The number of rows in the PDF417 code.

`columnCount`  

The number of columns in the PDF417 code.

## Return Value

A PDF417 code descriptor encoding the specified payload with the specified row and column counts.

## Discussion

The `CIBarcodeGenerator` filter can recreate a PDF417 code given the descriptor created using this method.

