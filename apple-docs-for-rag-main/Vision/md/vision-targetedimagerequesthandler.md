

- Vision
-  TargetedImageRequestHandler 

Class

# TargetedImageRequestHandler

An object that performs image-analysis requests on two images.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
final class TargetedImageRequestHandler
```

## Topics

### Creating a request handler

convenience init(sourceURL: URL, targetURL: URL, orientation: CGImagePropertyOrientation?)

Creates a handler for performing requests on an image at the specified URL.

convenience init(source: Data, target: Data, orientation: CGImagePropertyOrientation?)

Creates a handler for performing requests on an image contained in a data object.

convenience init(source: CGImage, target: CGImage, orientation: CGImagePropertyOrientation?)

Creates a handler for performing requests on Core Graphics images.

convenience init(source: CVPixelBuffer, target: CVPixelBuffer, orientation: CGImagePropertyOrientation?)

Creates a handler for performing requests on a Core Video pixel buffer.

convenience init(source: CMSampleBuffer, target: CMSampleBuffer, orientation: CGImagePropertyOrientation?)

Creates a request handler that performs requests on an image contained within a sample buffer.

convenience init(source: CIImage, target: CIImage, orientation: CGImagePropertyOrientation?)

Creates a handler for performing requests on Core Image images.

### Performing the request

func perform&lt;each T>(repeat each T) async throws -> (repeat (each T).Result)

Performs one or more framework requests on the handler’s image.

func perform&lt;T>(T) async throws -> T.Result

Performs a framework request on the handler’s image.

func performAll(some Collection&lt;any TargetedRequest>) -> some AsyncSequence&lt;VisionResult, Never> 

Schedules a collection of framework requests to perform on the handler’s image.

## Relationships

### Conforms To

- Sendable

## See Also

### Request Handlers

class ImageRequestHandler

An object that processes one or more image-analysis requests pertaining to a single image.

