

- Vision
- VNBarcodeObservation
-  barcodeDescriptor 

Instance Property

# barcodeDescriptor

An object that describes the low-level details about the barcode and its data.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var barcodeDescriptor: CIBarcodeDescriptor? { get }
```

## Discussion

Use this object to have Core Image regenerate the observed barcode.

