

- Core Image
-  CITextFeature 

Class

# CITextFeature

Information about a region likely to contain text detected in a still or video image.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class CITextFeature : CIFeature
```

## Overview

Note

In macOS 10.13, iOS 11, and tvOS 11 or later, the Vision framework replaces these classes for identifying and analyzing image features. See VNRecognizeTextRequest.

The properties of a `CITextFeature` object identify its corners in image coordinates. Use this class to locate areas of text within an image — for example, to extract and perspective-correct those portions of the image before performing your own optical character recognition or other processing tasks.

To detect rectangles in an image or video, choose the CIDetectorTypeText type when initializing a CIDetector object, and use the CIDetectorImageOrientation option to specify the desired orientation for finding upright text.

## Topics

### Locating a Detected Feature

var bounds: CGRect

A rectangle indicating the position and extent of the feature in image coordinates.

### Locating Features Within a Detected Region

var subFeatures: [Any]?

An array containing additional features detected within the feature.

### Identifying the Corners of a Detected Text Region

var bottomLeft: CGPoint

The lower-left corner of the detected text region, in image coordinates.

var bottomRight: CGPoint

The lower-right corner of the detected text region, in image coordinates.

var topLeft: CGPoint

The upper-left corner of the detected text region, in image coordinates.

var topRight: CGPoint

The upper-right corner of the detected text region, in image coordinates.

## Relationships

### Inherits From

- CIFeature

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

class CIQRCodeFeature

Information about a Quick Response code detected in a still or video image.

