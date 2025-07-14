

- AVFoundation
- AVAssetImageGenerator
-  images(for:) 

Instance Method

# images(for:)

Generates images for times within the video timeline.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func images(for times: [CMTime]) -> AVAssetImageGenerator.Images
```

## Parameters 

`times`  

An array of times within the asset timeline to create images.

## Return Value

An asynchronous sequence of images.

## Mentioned in 

Creating images from a video asset

## Topics

### Generated Image Sequence

struct Images

An asynchronous sequence of images created by an image generator.

## See Also

### Generating Images

func image(at: CMTime) async throws -> (image: CGImage, actualTime: CMTime)

Generates an image for a requested time.

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

