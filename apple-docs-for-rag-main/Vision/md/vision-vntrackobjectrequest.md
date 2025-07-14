

- Vision
-  VNTrackObjectRequest 

Class

# VNTrackObjectRequest

An image-analysis request that tracks the movement of a previously identified object across multiple images or video frames.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class VNTrackObjectRequest
```

## Overview

Use this type of request to track the bounding boxes around objects previously identified in an image. Vision attempts to locate the same object from the input observation throughout the sequence.

## Topics

### Initializing an Object Tracking Request

init(detectedObjectObservation: VNDetectedObjectObservation)

Creates a new object tracking request with a detected object observation.

init(detectedObjectObservation: VNDetectedObjectObservation, completionHandler: VNRequestCompletionHandler?)

Creates a new object tracking request with a detected object observation.

### Identifying Request Revisions

let VNTrackObjectRequestRevision2: Int

A constant for specifying revision 2 of the object tracking request.

let VNTrackObjectRequestRevision1: Int

A constant for specifying revision 1 of the object tracking request.

## Relationships

### Inherits From

- VNTrackingRequest

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

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

class VNDetectedObjectObservation

An observation that provides the position and extent of an image feature that an image- analysis request detects.

