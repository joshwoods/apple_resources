

- AVFoundation
- AVAssetImageGenerator
- AVAssetImageGenerator.Images
- AVAssetImageGenerator.Images.Element
-  image 

Instance Property

# image

An image for a requested time.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var image: CGImage { get throws }
```

## See Also

### Accessing Image Data

var requestedTime: CMTime

A time in the video timeline at which you request an image.

var actualTime: CMTime

The actual time in the video timeline at which the image generator creates the image.

