

- Core Image
-  CIRectangleFeature 

Class

# CIRectangleFeature

Information about a rectangular region detected in a still or video image.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
class CIRectangleFeature : CIFeature
```

## Overview

Note

In macOS 10.13, iOS 11, and tvOS 11 or later, the Vision framework replaces these classes for identifying and analyzing image features. See VNDetectRectanglesRequest.

A detected rectangle feature isn’t necessarily rectangular in the plane of the image; rather, the feature identifies a shape that may be rectangular in space but which appears in perspective in the image — for example, a paper or book on a desk. The properties of a `CIRectangleFeature` object identify its corners in image coordinates.

For example, you can use rectangle feature detection together with the CIPerspectiveCorrection filter to detect rectangular objects in an image or video and transform them to their original orientation.

To detect rectangles in an image or video, choose the CIDetectorTypeRectangle type when initializing a CIDetector object, and use the CIDetectorAspectRatio and CIDetectorFocalLength options to specify the approximate shape of rectangular features to search for. The detector returns at most one rectangle feature, the most prominent found in the image.

## Topics

### Locating a Detected Feature

var bounds: CGRect

A rectangle indicating the position and extent of the feature in image coordinates.

### Identifying the Corners of a Detected Rectangle

var bottomLeft: CGPoint

The lower-left corner of the detected rectangle, in image coordinates.

var bottomRight: CGPoint

The lower-right corner of the detected rectangle, in image coordinates.

var topLeft: CGPoint

The upper-left corner of the detected rectangle, in image coordinates.

var topRight: CGPoint

The upper-right corner of the detected rectangle, in image coordinates.

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

class CITextFeature

Information about a region likely to contain text detected in a still or video image.

class CIQRCodeFeature

Information about a Quick Response code detected in a still or video image.

