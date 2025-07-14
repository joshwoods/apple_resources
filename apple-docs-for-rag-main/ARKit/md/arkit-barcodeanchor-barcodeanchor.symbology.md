

- ARKit
- BarcodeAnchor
-  BarcodeAnchor.Symbology 

Enumeration

# BarcodeAnchor.Symbology

Values that describe specific kinds of barcodes.

visionOS 2.0+

``` source
enum Symbology
```

## Topics

### Barcode symbologies

case aztec

The value that represents the Aztec barcode symbology.

case codabar

The value that represents the Codabar barcode symbology.

case code128

The value that represents the Code 128 barcode symbology.

case code39

The value that represents the Code 39 barcode symbology.

case code39Checksum

The value that represents the Code 39 checksum barcode symbology.

case code39FullAscii

The value that represents the Code 39 full ASCII barcode symbology.

case code39FullAsciiChecksum

The value that represents the Code 39 full ASCII checksum barcode symbology.

case code93

The value that represents the Code 93 symbology.

case code93i

The value that represents the Code 93i barcode symbology.

case dataMatrix

The value that represents the Data Matrix barcode symbology.

case ean13

The value that represents the EAN13 barcode symbology.

case ean8

The value that represents the EAN8 barcode symbology.

case gs1DataBar

The value that represents the GS1 DataBar barcode symbology.

case gs1DataBarExpanded

The value that represents the GS1 DataBar Expanded barcode symbology.

case gs1DataBarLimited

The value that represents the GS1 DataBar Limited barcode symbology.

case itf

The value that represents the ITF barcode symbology.

case itf14

The value that represents the ITF14 barcode symbology.

case itfChecksum

The value that represents the ITF checksum barcode symbology.

case microPDF417

The value that represents the Micro PDF417 barcode symbology.

case microQR

The value that represents the Micro QR barcode symbology.

case msiPlessey

The value that represents the MSI Plessy barcode symbology.

case pdf417

The value that represents the PDF417 barcode symbology.

case qr

The value that represents the QR barcode symbology.

case upce

The value that represents the UPCE barcode symbology.

### Instance Properties

var description: String

A textual representation of BarcodeAnchor.Symbology

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Getting barcode information

var extent: SIMD3&lt;Float>

The extent of the detected barcode’s bounds.

var originFromAnchorTransform: simd_float4x4

The transform from the barcode anchor to the origin coordinate system.

var payloadData: Data

The encoded payload data of the detected barcode.

var payloadString: String?

The decoded payload string value of the detected barcode.

var symbology: BarcodeAnchor.Symbology

The symbology of the detected barcode.

var id: UUID

The unique identifier of an anchor.

