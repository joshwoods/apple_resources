

- Metal
- MTLBlitOption
-  stencilFromDepthStencil 

Type Property

# stencilFromDepthStencil

A blit option that copies the stencil portion of a combined depth and stencil texture to or from a buffer.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
static var stencilFromDepthStencil: MTLBlitOption { get }
```

## Discussion

You can pass this option to some methods that copy data between a buffer and a texture, including the following:

- copy(from:sourceOffset:sourceBytesPerRow:sourceBytesPerImage:sourceSize:to:destinationSlice:destinationLevel:destinationOrigin:options:)

- copy(from:sourceSlice:sourceLevel:sourceOrigin:sourceSize:to:destinationOffset:destinationBytesPerRow:destinationBytesPerImage:options:)

## See Also

### Depth and Stencil Buffer Options

static var depthFromDepthStencil: MTLBlitOption

A blit option that copies the depth portion of a combined depth and stencil texture to or from a buffer.

