

- Vision
-  VNSequenceRequestHandler 

Class

# VNSequenceRequestHandler

An object that processes image-analysis requests for each frame in a sequence.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class VNSequenceRequestHandler
```

## Overview

Instantiate this handler to perform Vision requests on a series of images. Unlike the VNImageRequestHandler, you don’t specify the image on creation. Instead, you supply each image frame one by one as you continue to call one of the `perform` methods.

## Topics

### Initializing a Sequence Request

init()

Initializes a sequence request handler.

### Performing a Sequence Request

func perform([VNRequest], on: CGImage) throws

Schedules Vision requests to be performed on a Core Graphics image.

func perform([VNRequest], on: CGImage, orientation: CGImagePropertyOrientation) throws

Schedules one or more Vision requests to be performed on a Core Graphics image with known orientation.

func perform([VNRequest], on: CIImage) throws

Schedules one or more Vision requests to be performed on Core Image image data.

func perform([VNRequest], on: CIImage, orientation: CGImagePropertyOrientation) throws

Schedules one or more Vision requests to be performed on Core Image image data with known orientation.

func perform([VNRequest], on: CVPixelBuffer) throws

Schedules one or more Vision requests to be performed on a Core Video pixel buffer.

func perform([VNRequest], on: CVPixelBuffer, orientation: CGImagePropertyOrientation) throws

Schedules one or more Vision requests to be performed on a Core Video pixel buffer with known orientation.

func perform([VNRequest], on: CMSampleBuffer) throws

Performs one or more requests on an image contained within a sample buffer.

func perform([VNRequest], on: CMSampleBuffer, orientation: CGImagePropertyOrientation) throws

Performs one or more requests on an image of a specified orientation contained within a sample buffer.

func perform([VNRequest], onImageData: Data) throws

Schedules one or more Vision requests to be performed on raw image data.

func perform([VNRequest], onImageData: Data, orientation: CGImagePropertyOrientation) throws

Schedules one or more Vision requests to be performed on raw data containing an image with known orientation.

func perform([VNRequest], onImageURL: URL) throws

Schedules one or more Vision requests to be performed on an image.

func perform([VNRequest], onImageURL: URL, orientation: CGImagePropertyOrientation) throws

Schedules one or more Vision requests to be performed on an image with known orientation, at a specific URL.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
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

class VNGeneratePersonSegmentationRequest

An object that produces a matte image for a person it finds in the input image.

class VNGeneratePersonInstanceMaskRequest

An object that produces a mask of individual people it finds in the input image.

class VNDetectDocumentSegmentationRequest

An object that detects rectangular regions that contain text in the input image.

