

- Core Image
- CIImageProcessorOutput
-  region 

Instance Property

# region

The rectangular region of the output image that your processor must provide.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var region: CGRect { get }
```

**Required**

## Discussion

Your image processor block may be invoked multiple times to provide output for multiple regions, and the region for which output is needed may not match the bounds of the output buffer, texture, or surface.

## See Also

### Getting Supplemental Information for Image Processing

var metalCommandBuffer: (any MTLCommandBuffer)?

A command buffer to use for image processing using Metal.

**Required**

var bytesPerRow: Int

The number of bytes per row of pixels for the output image.

**Required**

var format: CIFormat

The per-pixel data format expected of the output image.

**Required**

