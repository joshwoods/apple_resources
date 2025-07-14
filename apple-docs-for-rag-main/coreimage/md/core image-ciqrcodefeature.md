

- Core Image
-  CIQRCodeFeature 

Class

# CIQRCodeFeature

Information about a Quick Response code detected in a still or video image.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
class CIQRCodeFeature : CIFeature
```

## Overview

Note

In macOS 10.13, iOS 11, and tvOS 11 or later, the Vision framework replaces these classes for identifying and analyzing image features. See VNDetectBarcodesRequest.

A QR code is a two-dimensional barcode using the ISO/IEC 18004:2006 standard. The properties of a `CIQRCodeFeature` object identify the corners of the barcode in the image perspective and provide the decoded message.

To detect QR codes in an image or video, choose the CIDetectorTypeQRCode type when initializing a CIDetector object.

## Topics

### Locating a Detected Feature

var bounds: CGRect

A rectangle indicating the position and extent of the feature in image coordinates.

### Decoding a Detected Barcode

var messageString: String?

The string decoded from the detected barcode.

var symbolDescriptor: CIQRCodeDescriptor?

An abstract representation of a QR Code symbol.

### Identifying the Corners of a Detected Barcode

var bottomLeft: CGPoint

The lower-left corner of the detected barcode, in image coordinates.

var bottomRight: CGPoint

The lower-right corner of the detected barcode, in image coordinates.

var topLeft: CGPoint

The upper-left corner of the detected barcode, in image coordinates.

var topRight: CGPoint

The upper-right corner of the detected barcode, in image coordinates.

## Relationships

### Inherits From

- CIFeature

### Conforms To

- NSCopying
- NSSecureCoding

## See Also

### Image Feature Detection

class CIDetector

An image processor that identifies notable features, such as faces and barcodes, in a still image or video.

class CIFeature

The abstract superclass for objects representing notable features detected in an image.

class CIFaceFeature

Information about a face detected in a still or video image.

class CIRectangleFeature

Information about a rectangular region detected in a still or video image.

class CITextFeature

Information about a region likely to contain text detected in a still or video image.

