

- Vision
-  VNBarcodeSymbology 

Structure

# VNBarcodeSymbology

The barcode symbologies that the framework detects.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
struct VNBarcodeSymbology
```

## Discussion

Use supportedSymbologies() to get the specific symbologies the request supports.

## Topics

### Supported Symbologies

static let aztec: VNBarcodeSymbology

A constant that indicates Aztec symbology.

static let codabar: VNBarcodeSymbology

A constant that indicates Codabar symbology.

static let code39: VNBarcodeSymbology

A constant that indicates Code 39 symbology.

static let code39Checksum: VNBarcodeSymbology

A constant that indicates Code 39 symbology with a checksum.

static let code39FullASCII: VNBarcodeSymbology

A constant that indicates Code 39 Full ASCII symbology.

static let code39FullASCIIChecksum: VNBarcodeSymbology

A constant that indicates Code 39 Full ASCII symbology with a checksum.

static let code93: VNBarcodeSymbology

A constant that indicates Code 93 symbology.

static let code93i: VNBarcodeSymbology

A constant that indicates Code 93i symbology.

static let code128: VNBarcodeSymbology

A constant that indicates Code 128 symbology.

static let dataMatrix: VNBarcodeSymbology

A constant that indicates Data Matrix symbology.

static let ean8: VNBarcodeSymbology

A constant that indicates EAN-8 symbology.

static let ean13: VNBarcodeSymbology

A constant that indicates EAN-13 symbology.

static let gs1DataBar: VNBarcodeSymbology

A constant that indicates GS1 DataBar symbology.

static let gs1DataBarExpanded: VNBarcodeSymbology

A constant that indicates GS1 DataBar Expanded symbology.

static let gs1DataBarLimited: VNBarcodeSymbology

A constant that indicates GS1 DataBar Limited symbology.

static let i2of5: VNBarcodeSymbology

A constant that indicates Interleaved 2 of 5 (ITF) symbology.

static let i2of5Checksum: VNBarcodeSymbology

A constant that indicates Interleaved 2 of 5 (ITF) symbology with a checksum.

static let itf14: VNBarcodeSymbology

A constant that indicates ITF-14 symbology.

static let microPDF417: VNBarcodeSymbology

A constant that indicates MicroPDF417 symbology.

static let microQR: VNBarcodeSymbology

A constant that indicates MicroQR symbology.

static let msiPlessey: VNBarcodeSymbology

A constant that indicates Modified Plessey symbology.

static let pdf417: VNBarcodeSymbology

A constant that indicates PDF417 symbology.

static let qr: VNBarcodeSymbology

A constant that indicates Quick Response (QR) symbology.

static let upce: VNBarcodeSymbology

A constant that indicates UPC-E symbology.

### Deprecated Symbols

static var Aztec: VNBarcodeSymbology

A constant that indicates Aztec symbology.

Deprecated

static var Code128: VNBarcodeSymbologyDeprecated

static var Code39: VNBarcodeSymbology

A constant that indicates Code 39 symbology.

Deprecated

static var Code39Checksum: VNBarcodeSymbology

A constant that indicates Code 39 symbology with a checksum.

Deprecated

static var Code39FullASCII: VNBarcodeSymbology

A constant that indicates Code 39 Full ASCII symbology.

Deprecated

static var Code39FullASCIIChecksum: VNBarcodeSymbology

A constant that indicates Code 39 Full ASCII symbology with a checksum.

Deprecated

static var Code93: VNBarcodeSymbology

A constant that indicates Code 93 symbology.

Deprecated

static var Code93i: VNBarcodeSymbology

A constant that indicates Code 93i symbology.

Deprecated

static var DataMatrix: VNBarcodeSymbology

A constant that indicates Data Matrix symbology.

Deprecated

static var EAN8: VNBarcodeSymbology

A constant that indicates EAN-8 symbology.

Deprecated

static var EAN13: VNBarcodeSymbology

A constant that indicates EAN-13 symbology.

Deprecated

static var I2of5: VNBarcodeSymbology

A constant that indicates Interleaved 2 of 5 (ITF) symbology.

Deprecated

static var I2of5Checksum: VNBarcodeSymbology

A constant that indicates Interleaved 2 of 5 (ITF) symbology with a checksum.

Deprecated

static var ITF14: VNBarcodeSymbology

A constant that indicates ITF-14 symbology.

Deprecated

static var PDF417: VNBarcodeSymbology

A constant that indicates PDF417 symbology.

Deprecated

static var QR: VNBarcodeSymbology

A constant that indicates Quick Response (QR) symbology.

Deprecated

static var UPCE: VNBarcodeSymbology

A constant that indicates UPC-E symbology.

Deprecated

### Initializers

init(rawValue: String)

Creates a symbology with a string value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Specifying Symbologies

func supportedSymbologies() throws -> [VNBarcodeSymbology]

Returns the barcode symbologies that the request supports.

var symbologies: [VNBarcodeSymbology]

The barcode symbologies that the request detects in an image.

var coalesceCompositeSymbologies: Bool

A Boolean value that indicates whether to coalesce multiple codes based on the symbology.

class var supportedSymbologies: [VNBarcodeSymbology]

The array of barcode symbologies that the request supports.

Deprecated

