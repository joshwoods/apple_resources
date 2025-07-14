

- AVFoundation
- AVAssetImageGenerator
-  generateCGImagesAsynchronously(forTimes:completionHandler:) 

Instance Method

# generateCGImagesAsynchronously(forTimes:completionHandler:)

Generates images asynchronously for an array of requested times, and returns the results in a callback.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func generateCGImagesAsynchronously(
    forTimes requestedTimes: [NSValue],
    completionHandler handler: @escaping AVAssetImageGeneratorCompletionHandler
)
```

## Parameters 

`requestedTimes`  

An array of times, contained in NSValue objects, in the video timeline for which to generate images.

`handler`  

A callback that the image generator invokes for each requested image time.

## Discussion

Swift clients should prefer the asynchronous `images(for:)` method instead.

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

func generateCGImageAsynchronously(for: CMTime, completionHandler: (CGImage?, CMTime, (any Error)?) -> Void)

Generates an image asynchronously for a requested time, and returns the result in a callback.

typealias AVAssetImageGeneratorCompletionHandler

A type alias for a closure that provides the result of an image generation request.

func cancelAllCGImageGeneration()

Cancels all pending image generation requests.

func copyCGImage(at: CMTime, actualTime: UnsafeMutablePointer&lt;CMTime>?) throws -> CGImage

Returns an image for the asset at or near a specified time.

Deprecated

