

- UIKit
- UIImageReader
- UIImageReader.Configuration
-  pixelsPerInch 

Instance Property

# pixelsPerInch

The integral scale that the image reader applies to the image.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOSwatchOS 10.0+

``` source
var pixelsPerInch: Double { get set }
```

## Discussion

The default value is `0` which indicates a `1.0` scale.

## See Also

### Configuration properties

var prefersHighDynamicRange: Bool

A Boolean value that indicates whether the image reader should decode the image as HDR when the type is capable of decoding in either SDR or HDR.

var preparesImagesForDisplay: Bool

A Boolean value that indicates whether the image reader prepares the image for display.

var preferredThumbnailSize: CGSize

The thumbnail size in pixels that the image reader makes the image.

