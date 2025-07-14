

- Vision
-  VNDetectFaceLandmarksRequest 

Class

# VNDetectFaceLandmarksRequest

An image-analysis request that finds facial features like eyes and mouth in an image.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class VNDetectFaceLandmarksRequest
```

## Overview

By default, a face landmarks request first locates all faces in the input image, then analyzes each to detect facial features.

If you’ve already located all the faces in an image, or want to detect landmarks in only a subset of the faces in the image, set the inputFaceObservations property to an array of VNFaceObservation objects representing the faces you want to analyze. You can either use face observations output by a VNDetectFaceRectanglesRequest or manually create VNFaceObservation instances with the bounding boxes of the faces you want to analyze.

## Topics

### Configuring a Face Landmarks Request

protocol VNFaceObservationAccepting

An image analysis request that operates on face observations.

### Accessing the Results

var results: [VNFaceObservation]?

The results of the face landmarks request.

class VNFaceObservation

Face or facial-feature information that an image analysis request detects.

### Locating Face Landmarks

var constellation: VNRequestFaceLandmarksConstellation

A variable that describes how a face landmarks request orders or enumerates the resulting features.

enum VNRequestFaceLandmarksConstellation

An enumeration of face landmarks in a constellation object.

### Identifying Request Revisions

class func revision(Int, supportsConstellation: VNRequestFaceLandmarksConstellation) -> Bool

Returns a Boolean value that indicates whether a revision supports a constellation.

let VNDetectFaceLandmarksRequestRevision3: Int

A constant for specifying revision 3 of the face landmarks detection request.

let VNDetectFaceLandmarksRequestRevision2: Int

A constant for specifying revision 2 of the face landmarks detection request.

let VNDetectFaceLandmarksRequestRevision1: Int

A constant for specifying revision 1 of the face landmarks detection request.

Deprecated

## Relationships

### Inherits From

- VNImageBasedRequest

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- VNFaceObservationAccepting

## See Also

### Face and body detection

Selecting a selfie based on capture quality

Compare face-capture quality in a set of images by using Vision.

class VNDetectFaceCaptureQualityRequest

A request that produces a floating-point number that represents the capture quality of a face in a photo.

class VNDetectFaceRectanglesRequest

A request that finds faces within an image.

class VNDetectHumanRectanglesRequest

A request that finds rectangular regions that contain people in an image.

class VNHumanObservation

An object that represents a person that the request detects.

