

- UIKit
- UIImageReader
- UIImageReader.Configuration
-  prefersHighDynamicRange 

Instance Property

# prefersHighDynamicRange

A Boolean value that indicates whether the image reader should decode the image as HDR when the type is capable of decoding in either SDR or HDR.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOSwatchOS 10.0+

``` source
var prefersHighDynamicRange: Bool { get set }
```

## Discussion

This property doesn’t affect images that only decode in either SDR or HDR. The default value depends on the system capabilities.

## See Also

### Related Documentation

Applying Apple HDR effect to your photos

You can decode and apply Apple’s HDR gain map to your own images.

### Configuration properties

var preparesImagesForDisplay: Bool

A Boolean value that indicates whether the image reader prepares the image for display.

var preferredThumbnailSize: CGSize

The thumbnail size in pixels that the image reader makes the image.

var pixelsPerInch: Double

The integral scale that the image reader applies to the image.

