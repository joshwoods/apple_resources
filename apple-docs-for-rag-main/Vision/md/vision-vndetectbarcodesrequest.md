

- Vision
-  VNDetectBarcodesRequest 

Class

# VNDetectBarcodesRequest

A request that detects barcodes in an image.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class VNDetectBarcodesRequest
```

## Overview

This request returns an array of VNBarcodeObservation objects, one for each barcode it detects.

## Topics

### Specifying Symbologies

func supportedSymbologies() throws -> [VNBarcodeSymbology]

Returns the barcode symbologies that the request supports.

var symbologies: [VNBarcodeSymbology]

The barcode symbologies that the request detects in an image.

var coalesceCompositeSymbologies: Bool

A Boolean value that indicates whether to coalesce multiple codes based on the symbology.

struct VNBarcodeSymbology

The barcode symbologies that the framework detects.

class var supportedSymbologies: [VNBarcodeSymbology]

The array of barcode symbologies that the request supports.

Deprecated

### Accessing the Results

var results: [VNBarcodeObservation]?

The results of a barcode detection request.

class VNBarcodeObservation

An object that represents barcode information that an image analysis request detects.

### Identifying Request Revisions

let VNDetectBarcodesRequestRevision3: Int

A constant for specifying revision 3 of the barcode detection request.

let VNDetectBarcodesRequestRevision2: Int

A constant for specifying revision 2 of the barcode detection request.

Deprecated

let VNDetectBarcodesRequestRevision1: Int

A constant for specifying revision 1 of the barcode detection request.

Deprecated

## Relationships

### Inherits From

- VNImageBasedRequest

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Barcode detection

enum VNBarcodeCompositeType

Composite types for barcode requests.

