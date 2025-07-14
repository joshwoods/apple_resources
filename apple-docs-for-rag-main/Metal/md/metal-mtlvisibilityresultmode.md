

- Metal
-  MTLVisibilityResultMode 

Enumeration

# MTLVisibilityResultMode

The mode that determines what, if anything, the GPU writes to the results buffer, after the GPU executes the render pass.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
enum MTLVisibilityResultMode
```

## Topics

### Constants

case disabled

The result doesn’t contain any data because visibility testing was disabled.

case boolean

The result records whether any samples passed depth and stencil tests.

case counting

The result records how many samples passed depth and stencil tests.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Related Documentation

func setVisibilityResultMode(MTLVisibilityResultMode, offset: Int)

Configures which visibility test the GPU runs and the destination for any results it generates.

**Required**

### Encoding a Render Pass

protocol MTLRenderCommandEncoder

An interface that encodes a render pass into a command buffer, including all its draw calls and configuration.

enum MTLTriangleFillMode

Specifies how to rasterize triangle and triangle strip primitives.

enum MTLWinding

The vertex winding rule that determines a front-facing primitive.

enum MTLCullMode

The mode that determines whether to perform culling and which type of primitive to cull.

enum MTLPrimitiveType

The geometric primitive type for drawing commands.

enum MTLIndexType

The index type for an index buffer that references vertices of geometric primitives.

enum MTLDepthClipMode

The mode that determines how to deal with fragments outside of the near or far planes.

