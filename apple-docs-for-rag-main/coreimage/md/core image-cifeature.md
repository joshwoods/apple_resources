

- Core Image
-  CIFeature 

Class

# CIFeature

The abstract superclass for objects representing notable features detected in an image.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
class CIFeature : NSObject
```

## Overview

Note

In macOS 10.13, iOS 11, and tvOS 11 or later, the Vision framework replaces these classes for identifying and analyzing image features. See VNObservation.

A `CIFeature` object represents a portion of an image that a detector believes matches its criteria. Subclasses of `CIFeature` typically hold additional information specific to the detector that discovered the feature.

## Topics

### Feature Properties

var bounds: CGRect

The rectangle that holds discovered feature.

var type: String

The type of feature that was discovered.

### Feature Types

let CIFeatureTypeFace: String

The discovered feature is a person’s face.

let CIFeatureTypeRectangle: String

The discovered feature is a rectangular object, though it might appear in perspective in the image.

let CIFeatureTypeQRCode: String

The discovered feature is a Quick Response code (2D barcode).

let CIFeatureTypeText: String

The discovered feature is a region likely to contain upright text.

## Relationships

### Inherits From

- NSObject

## See Also

### Image Feature Detection

class CIDetector

An image processor that identifies notable features, such as faces and barcodes, in a still image or video.

class CIFaceFeature

Information about a face detected in a still or video image.

class CIRectangleFeature

Information about a rectangular region detected in a still or video image.

class CITextFeature

Information about a region likely to contain text detected in a still or video image.

class CIQRCodeFeature

Information about a Quick Response code detected in a still or video image.

