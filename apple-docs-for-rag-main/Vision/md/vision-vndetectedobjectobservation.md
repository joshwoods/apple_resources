

- Vision
-  VNDetectedObjectObservation 

Class

# VNDetectedObjectObservation

An observation that provides the position and extent of an image feature that an image- analysis request detects.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class VNDetectedObjectObservation
```

## Overview

This class is the observation type that VNTrackObjectRequest generates. It represents an object that the Vision request detects and tracks.

## Topics

### Creating an Observation

convenience init(boundingBox: CGRect)

Creates an observation with a bounding box.

convenience init(requestRevision: Int, boundingBox: CGRect)

Creates an observation with a revision number and bounding box.

### Locating a Detected Object

var boundingBox: CGRect

The bounding box of the object that the request detects.

### Accessing an Image Mask

var globalSegmentationMask: VNPixelBufferObservation?

A resulting pixel buffer from a request to generate a segmentation mask for an image.

## Relationships

### Inherits From

- VNObservation

### Inherited By

- VNFaceObservation
- VNHumanObservation
- VNRecognizedObjectObservation
- VNRectangleObservation

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

### Object tracking

Tracking the User’s Face in Real Time

Detect and track faces from the selfie cam feed in real time.

Tracking Multiple Objects or Rectangles in Video

Apply Vision algorithms to track objects or rectangles throughout a video.

class VNTrackingRequest

The abstract superclass for image-analysis requests that track unique features across multiple images or video frames.

class VNTrackRectangleRequest

An image-analysis request that tracks movement of a previously identified rectangular object across multiple images or video frames.

class VNTrackObjectRequest

An image-analysis request that tracks the movement of a previously identified object across multiple images or video frames.

