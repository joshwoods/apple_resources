

- Core Image
-  CIPDF417CodeDescriptor 

Class

# CIPDF417CodeDescriptor

A concrete subclass of CIBarcodeDescriptor that represents a PDF417 symbol.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class CIPDF417CodeDescriptor : CIBarcodeDescriptor
```

## Overview

PDF417 is a stacked linear barcode symbol format used predominantly in transport, ID cards, and inventory management. Each pattern in the code comprises 4 bars and spaces, 17 units long.

## Topics

### Creating a Descriptor

init?(payload: Data, isCompact: Bool, rowCount: Int, columnCount: Int)

Initializes a descriptor that can be used as input to the `CIBarcodeGenerator` filter.

### Examining a Descriptor

var errorCorrectedPayload: Data

The error-corrected payload containing the data encoded in the PDF417 code.

var isCompact: Bool

A boolean value telling if the PDF417 code is compact.

var rowCount: Int

The number of rows in the PDF417 code.

var columnCount: Int

The number of columns in the PDF417 code.

## Relationships

### Inherits From

- CIBarcodeDescriptor

## See Also

### Barcode Descriptions

class CIBarcodeDescriptor

An abstract base class that represents a machine-readable code's attributes.

class CIQRCodeDescriptor

A concrete subclass of CIBarcodeDescriptor that represents a square QR code symbol.

class CIAztecCodeDescriptor

A concrete subclass of CIBarcodeDescriptor that represents an Aztec code symbol.

class CIDataMatrixCodeDescriptor

A concrete subclass of CIBarcodeDescriptor that represents a Data Matrix code symbol.

