

- AVFoundation
- AVMetadataObject
-  AVMetadataObject.ObjectType 

Structure

# AVMetadataObject.ObjectType

Constants that identify metadata object types.

iOS 6.0+iPadOS 6.0+Mac Catalyst 14.0+macOS 10.10+tvOS 9.0+

``` source
struct ObjectType
```

## Topics

### Barcodes

static let codabar: AVMetadataObject.ObjectType

A constant that identifies the Codabar symbology.

static let code39: AVMetadataObject.ObjectType

A constant that identifies the Code 39 symbology.

static let code39Mod43: AVMetadataObject.ObjectType

A constant that identifies the Code 39 mod 43 symbology.

static let code93: AVMetadataObject.ObjectType

A constant that identifies the Code 93 symbology.

static let code128: AVMetadataObject.ObjectType

A constant that identifies the Code 128 symbology.

static let ean8: AVMetadataObject.ObjectType

A constant that identifies the EAN-8 symbology.

static let ean13: AVMetadataObject.ObjectType

A constant that identifies the EAN-13 symbology.

static let gs1DataBar: AVMetadataObject.ObjectType

A constant that identifies the GS1 DataBar symbology.

static let gs1DataBarExpanded: AVMetadataObject.ObjectType

A constant that identifies the GS1 DataBar Expanded symbology.

static let gs1DataBarLimited: AVMetadataObject.ObjectType

A constant that identifies the GS1 DataBar Limited symbology.

static let interleaved2of5: AVMetadataObject.ObjectType

A constant that identifies the Interleaved 2 of 5 symbology.

static let itf14: AVMetadataObject.ObjectType

A constant that identifies the ITF14 symbology.

static let upce: AVMetadataObject.ObjectType

A constant that identifies the UPC-E symbology.

### 2D Codes

static let aztec: AVMetadataObject.ObjectType

A constant that identifies the Aztec symbology.

static let dataMatrix: AVMetadataObject.ObjectType

A constant that identifies the DataMatrix symbology.

static let microPDF417: AVMetadataObject.ObjectType

A constant that identifies the Micro PDF417 symbology.

static let microQR: AVMetadataObject.ObjectType

A constant that identifies the Micro QR symbology.

static let pdf417: AVMetadataObject.ObjectType

A constant that identifies the PDF417 symbology.

static let qr: AVMetadataObject.ObjectType

A constant that identifies the QR symbology.

### Bodies

static let humanBody: AVMetadataObject.ObjectType

A constant that identifies human body metadata.

static let humanFullBody: AVMetadataObject.ObjectType

A constant that identifies human full body metadata.

static let dogBody: AVMetadataObject.ObjectType

A constant that identifies dog body metadata.

static let catBody: AVMetadataObject.ObjectType

A constant that identifies cat body metadata.

### Faces

static let face: AVMetadataObject.ObjectType

A constant that identifies face metadata.

### Saliency

static let salientObject: AVMetadataObject.ObjectType

A constant that identifies saliency metadata.

### Initializers

init(rawValue: String)

Creates a metadata object type with a string value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the Type of Metadata

var type: AVMetadataObject.ObjectType

The type of metadata that this object provides.

