

- Core Image
-  CIAztecCodeDescriptor 

Class

# CIAztecCodeDescriptor

A concrete subclass of CIBarcodeDescriptor that represents an Aztec code symbol.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class CIAztecCodeDescriptor : CIBarcodeDescriptor
```

## Overview

Aztec code is a format of 2D barcode published as ISO/IEC 24778:2008 standard. It encodes data in concentric square rings around a central bullseye pattern.

## Topics

### Creating a Descriptor

init?(payload: Data, isCompact: Bool, layerCount: Int, dataCodewordCount: Int)

Initializes a descriptor that can be used as input to the `CIBarcodeGenerator` filter.

### Examining a Descriptor

var errorCorrectedPayload: Data

The error-corrected payload containing the data encoded in the Aztec code.

var isCompact: Bool

A Boolean value telling if the Aztec code is compact.

var layerCount: Int

The number of layers embedded in the Aztec code.

var dataCodewordCount: Int

The number of data codewords in the Aztec code.

## Relationships

### Inherits From

- CIBarcodeDescriptor

## See Also

### Barcode Descriptions

class CIBarcodeDescriptor

An abstract base class that represents a machine-readable code's attributes.

class CIQRCodeDescriptor

A concrete subclass of CIBarcodeDescriptor that represents a square QR code symbol.

class CIPDF417CodeDescriptor

A concrete subclass of CIBarcodeDescriptor that represents a PDF417 symbol.

class CIDataMatrixCodeDescriptor

A concrete subclass of CIBarcodeDescriptor that represents a Data Matrix code symbol.

