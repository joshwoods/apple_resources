

- VisionKit
- RecognizedItem
-  RecognizedItem.Barcode 

Structure

# RecognizedItem.Barcode

An object that represents a machine-readable code that the scanner recognizes.

iOS 16.0+iPadOS 16.0+visionOS 1.0+

``` source
struct Barcode
```

## Topics

### Getting payloads

var payloadStringValue: String?

The payload or string representation for the barcode.

### Locating barcodes

var bounds: RecognizedItem.Bounds

The location of the recognized item in the view.

var observation: VNBarcodeObservation

A representation of the barcode information.

### Identifying barcodes

var id: UUID

A unique identifier for the recognized item.

## Relationships

### Conforms To

- Identifiable

## See Also

### Machine-readable items

case barcode(RecognizedItem.Barcode)

A machine-readable barcode.

