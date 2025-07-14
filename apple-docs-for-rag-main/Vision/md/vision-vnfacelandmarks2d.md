

- Vision
-  VNFaceLandmarks2D 

Class

# VNFaceLandmarks2D

A collection of facial features that a request detects.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class VNFaceLandmarks2D
```

## Overview

This class represents the set of all detectable 2D face landmarks and regions, exposed as properties. The coordinates of the face landmarks are normalized to the dimensions of the face observation’s boundingBox, with the origin at the bounding box’s lower-left corner. Use the VNImagePointForFaceLandmarkPoint(_:_:_:_:) function to convert normalized face landmark points into absolute points within the image’s coordinate system.

## Topics

### Face Landmark Points

var allPoints: VNFaceLandmarkRegion2D?

The region containing all face landmark points.

var faceContour: VNFaceLandmarkRegion2D?

The region containing points that trace the face contour from the left cheek, over the chin, to the right cheek.

var leftEye: VNFaceLandmarkRegion2D?

The region containing points that outline the left eye.

var rightEye: VNFaceLandmarkRegion2D?

The region containing points that outline the right eye.

var leftEyebrow: VNFaceLandmarkRegion2D?

The region containing points that trace the left eyebrow.

var rightEyebrow: VNFaceLandmarkRegion2D?

The region containing points that trace the right eyebrow.

var nose: VNFaceLandmarkRegion2D?

The region containing points that outline the nose.

var noseCrest: VNFaceLandmarkRegion2D?

The region containing points that trace the center crest of the nose.

var medianLine: VNFaceLandmarkRegion2D?

The region containing points that trace a vertical line down the center of the face.

var outerLips: VNFaceLandmarkRegion2D?

The region containing points that outline the outside of the lips.

var innerLips: VNFaceLandmarkRegion2D?

The region containing points that outline the space between the lips.

var leftPupil: VNFaceLandmarkRegion2D?

The region containing the point where the left pupil is located.

var rightPupil: VNFaceLandmarkRegion2D?

The region containing the point where the right pupil is located.

## Relationships

### Inherits From

- VNFaceLandmarks

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

class VNFaceLandmarkRegion2D

2D geometry information for a specific facial feature.

class VNFaceLandmarks

The abstract superclass for containers of face landmark information.

class VNFaceLandmarkRegion

The abstract superclass for information about a specific face landmark.

