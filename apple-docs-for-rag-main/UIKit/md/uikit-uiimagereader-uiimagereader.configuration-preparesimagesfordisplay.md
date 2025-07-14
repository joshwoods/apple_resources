

- UIKit
- UIImageReader
- UIImageReader.Configuration
-  preparesImagesForDisplay 

Instance Property

# preparesImagesForDisplay

A Boolean value that indicates whether the image reader prepares the image for display.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOSwatchOS 10.0+

``` source
var preparesImagesForDisplay: Bool { get set }
```

## Discussion

The default value is false.

## See Also

### Configuration properties

var prefersHighDynamicRange: Bool

A Boolean value that indicates whether the image reader should decode the image as HDR when the type is capable of decoding in either SDR or HDR.

var preferredThumbnailSize: CGSize

The thumbnail size in pixels that the image reader makes the image.

var pixelsPerInch: Double

The integral scale that the image reader applies to the image.

