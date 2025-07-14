

- Core Image
-  CIDetector 

Class

# CIDetector

An image processor that identifies notable features, such as faces and barcodes, in a still image or video.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
class CIDetector : NSObject
```

## Overview

Note

In macOS 10.13, iOS 11, and tvOS 11 or later, the Vision framework replaces these classes for identifying and analyzing image features. See VNRequest.

A `CIDetector` object uses image processing to search for and identify notable features (faces, rectangles, and barcodes) in a still image or video. Detected features are represented by CIFeature objects that provide more information about each feature.

This class can maintain many state variables that can impact performance. So for best performance, reuse `CIDetector` instances instead of creating new ones.

## Topics

### Creating a Detector Object

init?(ofType: String, context: CIContext?, options: [String : Any]?)

Creates and returns a configured detector.

### Using a Detector Object to Find Features

func features(in: CIImage) -> [CIFeature]

Searches for features in an image.

func features(in: CIImage, options: [String : Any]?) -> [CIFeature]

Searches for features in an image based on the specified image orientation.

### Constants

Detector Types

Strings used to declare the detector for which you are interested.

Detector Configuration Keys

Keys used in the options dictionary to configure a detector.

Detector Accuracy Options

Value options used to specify the desired accuracy of the detector.

Feature Detection Keys

Keys used in the options dictionary for features(in:options:).

## Relationships

### Inherits From

- NSObject

## See Also

### Image Feature Detection

class CIFeature

The abstract superclass for objects representing notable features detected in an image.

class CIFaceFeature

Information about a face detected in a still or video image.

class CIRectangleFeature

Information about a rectangular region detected in a still or video image.

class CITextFeature

Information about a region likely to contain text detected in a still or video image.

class CIQRCodeFeature

Information about a Quick Response code detected in a still or video image.

