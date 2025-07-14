

- Core Image
-  CIQRCodeDescriptor 

Class

# CIQRCodeDescriptor

A concrete subclass of CIBarcodeDescriptor that represents a square QR code symbol.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class CIQRCodeDescriptor : CIBarcodeDescriptor
```

## Overview

ISO/IEC 18004 defines versions from 1 to 40, where a higher symbol version indicates a larger data-carrying capacity.

QR codes can encode text, vCard contact information, or Uniform Resource Identifiers (URI).

## Topics

### Creating a Descriptor

init?(payload: Data, symbolVersion: Int, maskPattern: UInt8, errorCorrectionLevel: CIQRCodeDescriptor.ErrorCorrectionLevel)

Initializes a descriptor that can be used as input to the `CIBarcodeGenerator` filter.

### Examining a Descriptor

var errorCorrectedPayload: Data

The error-corrected payload containing the data encoded in the QR code.

var symbolVersion: Int

The version of the QR code.

var maskPattern: UInt8

The QR code's mask pattern.

var errorCorrectionLevel: CIQRCodeDescriptor.ErrorCorrectionLevel

The QR code error correction level.

### Error Correction Constants

enum CIQRCodeDescriptor.ErrorCorrectionLevel

Constants that indicate the percentage of the symbol dedicated to error correction.

## Relationships

### Inherits From

- CIBarcodeDescriptor

## See Also

### Barcode Descriptions

class CIBarcodeDescriptor

An abstract base class that represents a machine-readable code's attributes.

class CIAztecCodeDescriptor

A concrete subclass of CIBarcodeDescriptor that represents an Aztec code symbol.

class CIPDF417CodeDescriptor

A concrete subclass of CIBarcodeDescriptor that represents a PDF417 symbol.

class CIDataMatrixCodeDescriptor

A concrete subclass of CIBarcodeDescriptor that represents a Data Matrix code symbol.

