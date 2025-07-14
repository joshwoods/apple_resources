

- AVFoundation
- AVAssetImageGenerator
- AVAssetImageGenerator.Images
-  AVAssetImageGenerator.Images.Element 

Enumeration

# AVAssetImageGenerator.Images.Element

An element that provides the result of an image generation request.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
@frozen
enum Element
```

## Topics

### Cases

case success(requestedTime: CMTime, image: CGImage, actualTime: CMTime)

A result that indicates an image generation request succeeded.

case failure(requestedTime: CMTime, error: any Error)

A result that indicates an image generation request failed.

### Accessing Image Data

var image: CGImage

An image for a requested time.

var requestedTime: CMTime

A time in the video timeline at which you request an image.

var actualTime: CMTime

The actual time in the video timeline at which the image generator creates the image.

## Relationships

### Conforms To

- Sendable

## See Also

### Iterating Elements

func next() async -> AVAssetImageGenerator.Images.Element?

Returns the next element in the sequence.

