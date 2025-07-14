

- Vision
-  VNTrackingRequest 

Class

# VNTrackingRequest

The abstract superclass for image-analysis requests that track unique features across multiple images or video frames.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class VNTrackingRequest
```

## Overview

Instantiate a tracking request subclass to perform object tracking across multiple frames of an image. After initialization, configure the degree of accuracy by setting trackingLevel, and provide observations you’d like to track by setting the inputObservation initial bounding box.

## Topics

### Configuring a Tracking Request

enum VNRequestTrackingLevel

An enumeration of tracking priorities.

var inputObservation: VNDetectedObjectObservation

The observation object defining a region to track.

var trackingLevel: VNRequestTrackingLevel

A value for specifying whether to prioritize speed or location accuracy.

var isLastFrame: Bool

A Boolean that indicates the last frame in a tracking sequence.

### Getting the Number of Trackers

func supportedNumber(ofTrackersAndReturnError: NSErrorPointer) -> Int

Returns the maximum number of simultaneous trackers for the request.

## Relationships

### Inherits From

- VNImageBasedRequest

### Inherited By

- VNTrackObjectRequest
- VNTrackRectangleRequest

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

class VNTrackRectangleRequest

An image-analysis request that tracks movement of a previously identified rectangular object across multiple images or video frames.

class VNTrackObjectRequest

An image-analysis request that tracks the movement of a previously identified object across multiple images or video frames.

class VNDetectedObjectObservation

An observation that provides the position and extent of an image feature that an image- analysis request detects.

