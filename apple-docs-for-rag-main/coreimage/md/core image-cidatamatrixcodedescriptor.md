

- Core Image
-  CIDataMatrixCodeDescriptor 

Class

# CIDataMatrixCodeDescriptor

A concrete subclass of CIBarcodeDescriptor that represents a Data Matrix code symbol.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class CIDataMatrixCodeDescriptor : CIBarcodeDescriptor
```

## Overview

Data Matrix codes are two-dimensional barcodes comprising black and white cells arranged in a square or rectangular matrix pattern. They can encode text or numeric data.

## Topics

### Creating a Descriptor

init?(payload: Data, rowCount: Int, columnCount: Int, eccVersion: CIDataMatrixCodeDescriptor.ECCVersion)

Initializes a descriptor that can be used as input to the `CIBarcodeGenerator` filter.

### Examining a Descriptor

var errorCorrectedPayload: Data

The error-corrected payload that comprises the Data Matrix code symbol.

var rowCount: Int

The number of module rows.

var columnCount: Int

The number of module columns.

var eccVersion: CIDataMatrixCodeDescriptor.ECCVersion

The Data Matrix code ECC version.

### Error Correction Constants

enum CIDataMatrixCodeDescriptor.ECCVersion

Constants concerning Data Matrix code ECC version.

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

class CIPDF417CodeDescriptor

A concrete subclass of CIBarcodeDescriptor that represents a PDF417 symbol.

