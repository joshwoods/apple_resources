

- AVFoundation
- Additional data capture
- Metadata Types
- AVMetadataMachineReadableCodeObject
-  Machine-Readable Object Types 

API Collection

# Machine-Readable Object Types

Constants used to specify the type of barcode to scan.

## Overview

These constants are used in conjunction with the AVCaptureMetadataOutput class’s metadataObjectTypes property to specify the type (“symbology”) of barcode to scan. When a barcode is detected, the type property of `AVMetadataMachineReadableCodeObject` reflects the constant for the detected barcode’s symbology.

## Topics

### Constants

static let upce: AVMetadataObject.ObjectType

A constant that identifies the UPC-E symbology.

static let code39: AVMetadataObject.ObjectType

A constant that identifies the Code 39 symbology.

static let code39Mod43: AVMetadataObject.ObjectType

A constant that identifies the Code 39 mod 43 symbology.

static let ean13: AVMetadataObject.ObjectType

A constant that identifies the EAN-13 symbology.

static let ean8: AVMetadataObject.ObjectType

A constant that identifies the EAN-8 symbology.

static let code93: AVMetadataObject.ObjectType

A constant that identifies the Code 93 symbology.

static let code128: AVMetadataObject.ObjectType

A constant that identifies the Code 128 symbology.

static let pdf417: AVMetadataObject.ObjectType

A constant that identifies the PDF417 symbology.

static let qr: AVMetadataObject.ObjectType

A constant that identifies the QR symbology.

static let aztec: AVMetadataObject.ObjectType

A constant that identifies the Aztec symbology.

static let interleaved2of5: AVMetadataObject.ObjectType

A constant that identifies the Interleaved 2 of 5 symbology.

static let itf14: AVMetadataObject.ObjectType

A constant that identifies the ITF14 symbology.

static let dataMatrix: AVMetadataObject.ObjectType

A constant that identifies the DataMatrix symbology.

