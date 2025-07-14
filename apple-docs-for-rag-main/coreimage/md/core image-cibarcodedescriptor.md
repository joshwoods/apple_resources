

- Core Image
-  CIBarcodeDescriptor 

Class

# CIBarcodeDescriptor

An abstract base class that represents a machine-readable code's attributes.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class CIBarcodeDescriptor : NSObject
```

## Overview

Subclasses encapsulate the formal specification and fields specific to a code type. Each subclass is sufficient to recreate the unique symbol exactly as seen or used with a custom parser.

Listing 1 Creating a CIImage from a CIBarcodeDescriptor

## Relationships

### Inherits From

- NSObject

### Conforms To

- NSCopying
- NSSecureCoding

## See Also

### Barcode Descriptions

class CIQRCodeDescriptor

A concrete subclass of CIBarcodeDescriptor that represents a square QR code symbol.

class CIAztecCodeDescriptor

A concrete subclass of CIBarcodeDescriptor that represents an Aztec code symbol.

class CIPDF417CodeDescriptor

A concrete subclass of CIBarcodeDescriptor that represents a PDF417 symbol.

class CIDataMatrixCodeDescriptor

A concrete subclass of CIBarcodeDescriptor that represents a Data Matrix code symbol.

