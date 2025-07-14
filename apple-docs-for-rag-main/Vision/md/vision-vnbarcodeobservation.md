

- Vision
-  VNBarcodeObservation 

Class

# VNBarcodeObservation

An object that represents barcode information that an image analysis request detects.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class VNBarcodeObservation
```

## Overview

This type of observation results from a VNDetectBarcodesRequest. It contains information about the detected barcode, including parsed payload data for supported symbologies.

## Topics

### Parsing the Payload

var payloadStringValue: String?

A string value that represents the barcode payload.

var payloadData: Data?

The raw data representation of the barcode’s payload.

var supplementalPayloadString: String?

The supplemental code decoded as a string value.

var supplementalPayloadData: Data?

var supplementalCompositeType: VNBarcodeCompositeType

The supplemental composite type.

var isGS1DataCarrier: Bool

A Boolean value that indicates whether the barcode carries any global standards data.

### Reading Barcode Descriptors

var barcodeDescriptor: CIBarcodeDescriptor?

An object that describes the low-level details about the barcode and its data.

### Identifying Barcode Types

var symbology: VNBarcodeSymbology

The symbology of the observed barcode.

### Identifying Barcode Colors

var isColorInverted: Bool

A Boolean value that indicates whether the barcode is color inverted.

## Relationships

### Inherits From

- VNRectangleObservation

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- VNRequestRevisionProviding

## See Also

### Accessing the Results

var results: [VNBarcodeObservation]?

The results of a barcode detection request.

