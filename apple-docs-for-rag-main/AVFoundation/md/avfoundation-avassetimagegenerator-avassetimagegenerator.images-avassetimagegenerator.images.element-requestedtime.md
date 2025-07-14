

- AVFoundation
- AVAssetImageGenerator
- AVAssetImageGenerator.Images
- AVAssetImageGenerator.Images.Element
-  requestedTime 

Instance Property

# requestedTime

A time in the video timeline at which you request an image.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var requestedTime: CMTime { get }
```

## See Also

### Accessing Image Data

var image: CGImage

An image for a requested time.

var actualTime: CMTime

The actual time in the video timeline at which the image generator creates the image.

