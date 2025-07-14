

- AVFoundation
- AVAssetImageGenerator
-  copyCGImage(at:actualTime:) Deprecated

Instance Method

# copyCGImage(at:actualTime:)

Returns an image for the asset at or near a specified time.

iOS 4.0–18.0DeprecatediPadOS 4.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOS 9.0–18.0Deprecated

``` source
func copyCGImage(
    at requestedTime: CMTime,
    actualTime: UnsafeMutablePointer?
) throws -> CGImage
```

Deprecated

Use image(at:) instead or generateCGImagesAsynchronously(forTimes:completionHandler:).

## Parameters 

`requestedTime`  

A time within the asset timeline for which to create an image.

`actualTime`  

Upon return, contains the time at which the image was actually generated.

If you’re not interested in this information, pass `NULL`.

## Return Value

A CGImage for the asset at or near a specified time, or `NULL` if the image could not be created.

## Discussion

This method returns the image synchronously.

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

func cancelAllCGImageGeneration()

Cancels all pending image generation requests.

