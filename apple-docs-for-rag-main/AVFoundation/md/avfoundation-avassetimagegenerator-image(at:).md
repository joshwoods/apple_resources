

- AVFoundation
- AVAssetImageGenerator
-  image(at:) 

Instance Method

# image(at:)

Generates an image for a requested time.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func image(at time: CMTime) async throws -> (image: CGImage, actualTime: CMTime)
```

## Parameters 

`time`  

A time in the asset timeline at which to create an image.

## Return Value

A tuple that contains the image and the time the asset was created.

## Mentioned in 

Creating images from a video asset

## See Also

### Generating Images

func images(for: [CMTime]) -> AVAssetImageGenerator.Images

Generates images for times within the video timeline.

func generateCGImageAsynchronously(for: CMTime, completionHandler: (CGImage?, CMTime, (any Error)?) -> Void)

Generates an image asynchronously for a requested time, and returns the result in a callback.

func generateCGImagesAsynchronously(forTimes: [NSValue], completionHandler: AVAssetImageGeneratorCompletionHandler)

Generates images asynchronously for an array of requested times, and returns the results in a callback.

typealias AVAssetImageGeneratorCompletionHandler

A type alias for a closure that provides the result of an image generation request.

func cancelAllCGImageGeneration()

Cancels all pending image generation requests.

func copyCGImage(at: CMTime, actualTime: UnsafeMutablePointer&lt;CMTime>?) throws -> CGImage

Returns an image for the asset at or near a specified time.

Deprecated

