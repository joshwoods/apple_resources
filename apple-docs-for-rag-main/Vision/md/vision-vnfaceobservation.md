

- Vision
-  VNFaceObservation 

Class

# VNFaceObservation

Face or facial-feature information that an image analysis request detects.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class VNFaceObservation
```

## Overview

This type of observation results from a VNDetectFaceRectanglesRequest. It contains information about facial landmarks and regions it finds in the image.

## Topics

### Creating an Observation

convenience init(requestRevision: Int, boundingBox: CGRect, roll: NSNumber?, yaw: NSNumber?, pitch: NSNumber?)

Creates an observation that contains the roll, yaw, and pitch of the face.

convenience init(requestRevision: Int, boundingBox: CGRect, roll: NSNumber?, yaw: NSNumber?)

Creates an observation that contains the roll and yaw of the face.

Deprecated

### Identifying Landmarks

var landmarks: VNFaceLandmarks2D?

The facial features of the detected face.

class VNFaceLandmarks2D

A collection of facial features that a request detects.

class VNFaceLandmarkRegion2D

2D geometry information for a specific facial feature.

class VNFaceLandmarks

The abstract superclass for containers of face landmark information.

class VNFaceLandmarkRegion

The abstract superclass for information about a specific face landmark.

### Determining Facial Orientation

var roll: NSNumber?

The roll angle of a face in radians.

var yaw: NSNumber?

The yaw angle of a face in radians.

var pitch: NSNumber?

The pitch angle of a face in radians.

### Determining Capture Quality

var faceCaptureQuality: Float?

A value that indicates the quality of the face capture.

## Relationships

### Inherits From

- VNDetectedObjectObservation

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

### Accessing the Results

var results: [VNFaceObservation]?

The results of the face-capture quality request.

