

- UIKit
- UIImageReader
- UIImageReader.Configuration
-  preferredThumbnailSize 

Instance Property

# preferredThumbnailSize

The thumbnail size in pixels that the image reader makes the image.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOSwatchOS 10.0+

``` source
var preferredThumbnailSize: CGSize { get set }
```

## Discussion

The default value is CGSizeZero.

## See Also

### Configuration properties

var prefersHighDynamicRange: Bool

A Boolean value that indicates whether the image reader should decode the image as HDR when the type is capable of decoding in either SDR or HDR.

var preparesImagesForDisplay: Bool

A Boolean value that indicates whether the image reader prepares the image for display.

var pixelsPerInch: Double

The integral scale that the image reader applies to the image.

