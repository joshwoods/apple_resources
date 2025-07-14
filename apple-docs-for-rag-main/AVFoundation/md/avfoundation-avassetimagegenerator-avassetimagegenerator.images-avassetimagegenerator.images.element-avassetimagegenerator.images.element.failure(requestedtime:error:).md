

- AVFoundation
- AVAssetImageGenerator
- AVAssetImageGenerator.Images
- AVAssetImageGenerator.Images.Element
-  AVAssetImageGenerator.Images.Element.failure(requestedTime:error:) 

Case

# AVAssetImageGenerator.Images.Element.failure(requestedTime:error:)

A result that indicates an image generation request failed.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
case failure(
    requestedTime: CMTime,
    error: any Error
)
```

## Parameters 

`requestedTime`  

A time in the video timeline at which you requested an image.

`error`  

An error that indicates the reason for the failure.

## See Also

### Cases

case success(requestedTime: CMTime, image: CGImage, actualTime: CMTime)

A result that indicates an image generation request succeeded.

