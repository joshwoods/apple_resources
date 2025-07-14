

- AVFoundation
- AVAssetImageGenerator
-  cancelAllCGImageGeneration() 

Instance Method

# cancelAllCGImageGeneration()

Cancels all pending image generation requests.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
func cancelAllCGImageGeneration()
```

## Discussion

Calling this method invokes the handler block with a result of AVAssetImageGenerator.Result.cancelled for all requested times for which the generator hasn’t yet produced an image.

## See Also

### Generating Images

func image(at: CMTime) async throws -> (image: CGImage, actualTime: CMTime)

Generates an image for a requested time.

func images(for: [CMTime]) -> AVAssetImageGenerator.Images

Generates images for times within the video timeline.

func generateCGImageAsynchronously(for: CMTime, completionHandler: (CGImage?, CMTime, (any Error)?) -> Void)

Generates an image asynchronously for a requested time, and returns the result in a callback.

func generateCGImagesAsynchronously(forTimes: [NSValue], completionHandler: AVAssetImageGeneratorCompletionHandler)

Generates images asynchronously for an array of requested times, and returns the results in a callback.

typealias AVAssetImageGeneratorCompletionHandler

A type alias for a closure that provides the result of an image generation request.

func copyCGImage(at: CMTime, actualTime: UnsafeMutablePointer&lt;CMTime>?) throws -> CGImage

Returns an image for the asset at or near a specified time.

Deprecated

