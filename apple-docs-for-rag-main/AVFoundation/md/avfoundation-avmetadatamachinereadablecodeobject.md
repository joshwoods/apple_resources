

- AVFoundation
-  AVMetadataMachineReadableCodeObject 

Class

# AVMetadataMachineReadableCodeObject

Barcode information detected by a metadata capture output.

iOS 7.0+iPadOS 7.0+Mac Catalyst 14.0+macOS 10.15+tvOS 9.0+

``` source
class AVMetadataMachineReadableCodeObject
```

## Overview

The `AVMetadataMachineReadableCodeObject` class is a concrete subclass of AVMetadataObject defining the features of a detected one-dimensional or two-dimensional barcode.

An `AVMetadataMachineReadableCodeObject` instance represents a single detected machine readable code in an image.  It’s an immutable object describing the features and payload of a barcode.

On supported platforms, the AVCaptureMetadataOutput class outputs arrays of detected machine readable code objects.

## Topics

### Getting Machine Readable Code Values

var corners: [CGPoint]

A Swift array of corner points.

var descriptor: CIBarcodeDescriptor?

A barcode description for use in Core Image.

var stringValue: String?

Returns the error-corrected data decoded into a human-readable string.

### Constants

Machine-Readable Object Types

Constants used to specify the type of barcode to scan.

## Relationships

### Inherits From

- AVMetadataObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

