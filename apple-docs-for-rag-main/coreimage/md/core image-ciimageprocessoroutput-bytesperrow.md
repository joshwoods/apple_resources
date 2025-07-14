

- Core Image
- CIImageProcessorOutput
-  bytesPerRow 

Instance Property

# bytesPerRow

The number of bytes per row of pixels for the output image.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var bytesPerRow: Int { get }
```

**Required**

## See Also

### Getting Supplemental Information for Image Processing

var region: CGRect

The rectangular region of the output image that your processor must provide.

**Required**

var metalCommandBuffer: (any MTLCommandBuffer)?

A command buffer to use for image processing using Metal.

**Required**

var format: CIFormat

The per-pixel data format expected of the output image.

**Required**

