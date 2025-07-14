

- VisionKit
- DataScannerViewController
- DataScannerViewController.RecognizedDataType
-  barcode(symbologies:) 

Type Method

# barcode(symbologies:)

Creates a data type for barcodes the use the specified symbologies.

iOS 16.0+iPadOS 16.0+visionOS 1.0+

``` source
static func barcode(symbologies: [VNBarcodeSymbology] = []) -> DataScannerViewController.RecognizedDataType
```

## Parameters 

`symbologies`  

The barcode symbologies that the scanner recognizes.

## Return Value

A barcode data type for the specified symbologies.

