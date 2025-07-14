

- AVFoundation
- AVAssetImageGenerator
-  generateCGImageAsynchronously(for:completionHandler:) 

Instance Method

# generateCGImageAsynchronously(for:completionHandler:)

Generates an image asynchronously for a requested time, and returns the result in a callback.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func generateCGImageAsynchronously(
    for requestedTime: CMTime,
    completionHandler handler: @escaping (CGImage?, CMTime, (any Error)?) -> Void
)
```

## Parameters 

`requestedTime`  

A time in the video timeline for which to generate an image. The requested time and actual time at which it generates an image may differ depending on the generator’s time tolerance settings.

`handler`  

A callback that the image generator invokes with the result of the request.

## Discussion

Swift clients should use the asynchronous image(at:) method instead.

## Topics

### Data Types

typealias AVAssetImageGeneratorCompletionHandler

A type alias for a closure that provides the result of an image generation request.

enum Result

Constants that indicate the result of an image generation request.

## See Also

### Generating Images

func image(at: CMTime) async throws -> (image: CGImage, actualTime: CMTime)

Generates an image for a requested time.

func images(for: [CMTime]) -> AVAssetImageGenerator.Images

Generates images for times within the video timeline.

func generateCGImagesAsynchronously(forTimes: [NSValue], completionHandler: AVAssetImageGeneratorCompletionHandler)

Generates images asynchronously for an array of requested times, and returns the results in a callback.

typealias AVAssetImageGeneratorCompletionHandler

A type alias for a closure that provides the result of an image generation request.

func cancelAllCGImageGeneration()

Cancels all pending image generation requests.

func copyCGImage(at: CMTime, actualTime: UnsafeMutablePointer&lt;CMTime>?) throws -> CGImage

Returns an image for the asset at or near a specified time.

Deprecated

