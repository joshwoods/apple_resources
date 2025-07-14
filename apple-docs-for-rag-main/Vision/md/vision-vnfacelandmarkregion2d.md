

- Vision
-  VNFaceLandmarkRegion2D 

Class

# VNFaceLandmarkRegion2D

2D geometry information for a specific facial feature.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class VNFaceLandmarkRegion2D
```

## Overview

This class represents the set of all facial landmark regions in 2D, exposed as properties.

## Topics

### Describing Region Points

var pointsClassification: VNPointsClassification

An enumeration that describes how to interpret the points the region provides.

enum VNPointsClassification

The set of classifications that describe how to interpret the points the region provides.

### Specifying Region Properties

var normalizedPoints: [CGPoint]

The array of normalized landmark points.

var precisionEstimatesPerPoint: [Float]?

Requests an array of precision estimates for each landmark point.

### Computing Feature Points

func pointsInImage(imageSize: CGSize) -> [CGPoint]

Returns an array containing landmark points in the coordinate space of the specified image size.

## Relationships

### Inherits From

- VNFaceLandmarkRegion

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

### Identifying Landmarks

var landmarks: VNFaceLandmarks2D?

The facial features of the detected face.

class VNFaceLandmarks2D

A collection of facial features that a request detects.

class VNFaceLandmarks

The abstract superclass for containers of face landmark information.

class VNFaceLandmarkRegion

The abstract superclass for information about a specific face landmark.

