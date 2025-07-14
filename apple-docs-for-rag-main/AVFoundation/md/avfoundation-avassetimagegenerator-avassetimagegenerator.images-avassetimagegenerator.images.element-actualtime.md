

- AVFoundation
- AVAssetImageGenerator
- AVAssetImageGenerator.Images
- AVAssetImageGenerator.Images.Element
-  actualTime 

Instance Property

# actualTime

The actual time in the video timeline at which the image generator creates the image.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var actualTime: CMTime { get throws }
```

## Discussion

This value may differ from the requestedTime depending on the configuration of the image generator’s requestedTimeToleranceBefore and requestedTimeToleranceAfter properties.

## See Also

### Accessing Image Data

var image: CGImage

An image for a requested time.

var requestedTime: CMTime

A time in the video timeline at which you request an image.

