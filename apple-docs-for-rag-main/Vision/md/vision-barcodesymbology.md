

- Vision
-  BarcodeSymbology 

Enumeration

# BarcodeSymbology

The barcode symbologies that the framework detects.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
enum BarcodeSymbology
```

## Topics

### Getting the symbologies

case aztec

case codabar

case code128

case code39

case code39Checksum

case code39FullASCII

case code39FullASCIIChecksum

case code93

case code93i

case dataMatrix

case ean13

case ean8

case gs1DataBar

case gs1DataBarExpanded

case gs1DataBarLimited

case i2of5

case i2of5Checksum

case itf14

case microPDF417

case microQR

case msiPlessey

case pdf417

case qr

case upce

## Relationships

### Conforms To

- CaseIterable
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Inspecting a request

var symbologies: [BarcodeSymbology]

The barcode symbologies that the request detects in an image.

var supportedSymbologies: [BarcodeSymbology]

The collection of barcode symbologies that the request can recognize.

var coalescesCompositeSymbologies: Bool

A Boolean value that indicates whether the request coalesces multiple codes into one.

