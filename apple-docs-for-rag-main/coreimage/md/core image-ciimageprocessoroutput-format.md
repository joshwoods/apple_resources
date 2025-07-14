

- Core Image
- CIImageProcessorOutput
-  format 

Instance Property

# format

The per-pixel data format expected of the output image.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var format: CIFormat { get }
```

**Required**

## Discussion

Your image processing routine must provide data in this pixel format.

## See Also

### Getting Supplemental Information for Image Processing

var region: CGRect

The rectangular region of the output image that your processor must provide.

**Required**

var metalCommandBuffer: (any MTLCommandBuffer)?

A command buffer to use for image processing using Metal.

**Required**

var bytesPerRow: Int

The number of bytes per row of pixels for the output image.

**Required**

