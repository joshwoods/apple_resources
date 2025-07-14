

- AVFoundation
- AVAssetImageGenerator
- AVAssetImageGenerator.Images
- AVAssetImageGenerator.Images.Element
-  AVAssetImageGenerator.Images.Element.success(requestedTime:image:actualTime:) 

Case

# AVAssetImageGenerator.Images.Element.success(requestedTime:image:actualTime:)

A result that indicates an image generation request succeeded.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
case success(
    requestedTime: CMTime,
    image: CGImage,
    actualTime: CMTime
)
```

## Parameters 

`requestedTime`  

A time in the video timeline at which you requested an image.

`image`  

An image for the requested time.

`actualTime`  

A time in the video timeline at which the image generator created an image.

## See Also

### Cases

case failure(requestedTime: CMTime, error: any Error)

A result that indicates an image generation request failed.

