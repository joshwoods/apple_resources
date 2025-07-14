

- Core Image
- CIImageProcessorOutput
-  metalCommandBuffer 

Instance Property

# metalCommandBuffer

A command buffer to use for image processing using Metal.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var metalCommandBuffer: (any MTLCommandBuffer)? { get }
```

**Required**

## Discussion

If you perform image processing with a Metal shader (and write output to the metalTexture property), encode your render or compute commands to this buffer. Core Image uses the same command buffer to render other effects that precede or follow your processor in a filter chain.

## See Also

### Getting Supplemental Information for Image Processing

var region: CGRect

The rectangular region of the output image that your processor must provide.

**Required**

var bytesPerRow: Int

The number of bytes per row of pixels for the output image.

**Required**

var format: CIFormat

The per-pixel data format expected of the output image.

**Required**

