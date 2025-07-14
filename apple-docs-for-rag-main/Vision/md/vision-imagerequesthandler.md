

- Vision
-  ImageRequestHandler 

Class

# ImageRequestHandler

An object that processes one or more image-analysis requests pertaining to a single image.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
final class ImageRequestHandler
```

## Overview

Instantiate this handler to perform Vision requests on a single image. You specify the image, and then call perform(_:) to begin executing the request.

## Topics

### Creating a request handler

convenience init(URL, orientation: CGImagePropertyOrientation?)

Creates a handler for performing requests on an image at the specified URL.

convenience init(Data, orientation: CGImagePropertyOrientation?)

Creates a handler for performing requests on an image contained in a data object.

convenience init(CGImage, orientation: CGImagePropertyOrientation?)

Creates a handler for performing requests on Core Graphics images.

convenience init(CVPixelBuffer, depthData: AVDepthData?, orientation: CGImagePropertyOrientation?)

Creates a handler for performing requests on a Core Video pixel buffer.

convenience init(CMSampleBuffer, depthData: AVDepthData?, orientation: CGImagePropertyOrientation?)

Creates a request handler that performs requests on an image contained within a sample buffer.

convenience init(CIImage, orientation: CGImagePropertyOrientation?)

Creates a handler for performing requests on Core Image images.

### Performing the request

func perform&lt;each T>(repeat each T) async throws -> (repeat (each T).Result)

Performs one or more framework requests on the handler’s image.

func perform&lt;T>(T) async throws -> T.Result

Performs a framework request on the handler’s image.

func performAll(some Collection&lt;any VisionRequest>) -> some AsyncSequence&lt;VisionResult, Never> 

Schedules a collection of framework requests to perform on the handler’s image.

## Relationships

### Conforms To

- Sendable

## See Also

### Still-image analysis

Classifying images for categorization and search

Analyze and label images using a Vision classification request.

struct ClassifyImageRequest

A request to classify an image.

protocol ImageProcessingRequest

A type for image-analysis requests that focus on a specific part of an image.

protocol VisionRequest

A type for image-analysis requests.

protocol VisionObservation

A type for objects produced by image-analysis requests.

