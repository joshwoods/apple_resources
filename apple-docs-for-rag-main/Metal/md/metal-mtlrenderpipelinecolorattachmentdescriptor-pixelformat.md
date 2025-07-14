

- Metal
- MTLRenderPipelineColorAttachmentDescriptor
-  pixelFormat 

Instance Property

# pixelFormat

The pixel format of the color attachment’s texture.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var pixelFormat: MTLPixelFormat { get set }
```

## Discussion

The pixel format of the rendering pipeline state must be set to match the pixel format of the texture used by the selected color attachment; otherwise, an error occurs.

## See Also

### Related Documentation

Metal Shading Language Guide

Metal Programming Guide

### Specifying Render Pipeline State

var writeMask: MTLColorWriteMask

A bitmask that restricts which color channels are written into the texture.

