

- AVFoundation
-  AVAssetImageGeneratorCompletionHandler 

Type Alias

# AVAssetImageGeneratorCompletionHandler

A type alias for a closure that provides the result of an image generation request.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias AVAssetImageGeneratorCompletionHandler = (CMTime, CGImage?, CMTime, AVAssetImageGenerator.Result, (any Error)?) -> Void
```

## Parameters 

`requestedTime`  

A time in the video timeline for which to generate an image.

`image`  

A generated image for the requested time.

`actualTime`  

The actual time in the video timeline at which it generated an image. The requested and actual times may differ depending on your image generator configuration including its time tolerance values.

`result`  

A value that indicates the result of the image generation request.

`error`  

An optional error. If an error occurs the system provides an error object that provides the details of the failure.

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

func cancelAllCGImageGeneration()

Cancels all pending image generation requests.

func copyCGImage(at: CMTime, actualTime: UnsafeMutablePointer&lt;CMTime>?) throws -> CGImage

Returns an image for the asset at or near a specified time.

Deprecated

