

- Vision
-  VNGeneratePersonSegmentationRequest 

Class

# VNGeneratePersonSegmentationRequest

An object that produces a matte image for a person it finds in the input image.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
class VNGeneratePersonSegmentationRequest
```

## Overview

Perform this request to detect and generate an image mask for a person in an image. The request returns the resulting image mask in an instance of VNPixelBufferObservation.

## Topics

### Creating a Request

init()

Creates a generate person segmentation request.

init(completionHandler: VNRequestCompletionHandler?)

Creates a generate person segmentation request with a completion handler.

### Configuring the Request

var outputPixelFormat: OSType

The pixel format of the output image.

var qualityLevel: VNGeneratePersonSegmentationRequest.QualityLevel

A value that indicates how the request balances accuracy and performance.

enum QualityLevel

Constants that define the levels of quality for a person segmentation request.

### Accessing the Results

var results: [VNPixelBufferObservation]?

The results of the segmentation request.

class VNPixelBufferObservation

An object that represents an image that an image-analysis request produces.

### Identifying Request Revisions

let VNGeneratePersonSegmentationRequestRevision1: Int

A constant for specifying revision 1 of the person segmentation generation request.

### Instance Methods

func supportedOutputPixelFormats() throws -> [NSNumber]

Returns a list of output pixel formats that the request supports.

## Relationships

### Inherits From

- VNStatefulRequest

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Image sequence analysis

Applying Matte Effects to People in Images and Video

Generate image masks for people automatically by using semantic person-segmentation.

Detecting Human Actions in a Live Video Feed

Identify body movements by sending a person’s pose data from a series of video frames to an action-classification model.

Segmenting and colorizing individuals from a surrounding scene

Use the Vision framework to isolate and apply colors to people in an image.

class VNStatefulRequest

An abstract request type that builds evidence of a condition over time.

class VNGeneratePersonInstanceMaskRequest

An object that produces a mask of individual people it finds in the input image.

class VNDetectDocumentSegmentationRequest

An object that detects rectangular regions that contain text in the input image.

class VNSequenceRequestHandler

An object that processes image-analysis requests for each frame in a sequence.

