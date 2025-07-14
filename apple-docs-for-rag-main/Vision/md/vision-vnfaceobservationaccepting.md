

- Vision
-  VNFaceObservationAccepting 

Protocol

# VNFaceObservationAccepting

An image analysis request that operates on face observations.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
protocol VNFaceObservationAccepting : NSObjectProtocol
```

## Overview

This protocol allows you to provide an input collection of VNFaceObservation objects as part of a request. Request objects adopt this protocol to request additional information about detected faces, such as facial landmarks.

## Topics

### Providing Face Observations

var inputFaceObservations: [VNFaceObservation]?

An array of VNFaceObservation objects to process as part of the request.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- VNDetectFaceCaptureQualityRequest
- VNDetectFaceLandmarksRequest

