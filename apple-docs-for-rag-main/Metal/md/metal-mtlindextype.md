

- Metal
-  MTLIndexType 

Enumeration

# MTLIndexType

The index type for an index buffer that references vertices of geometric primitives.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
enum MTLIndexType
```

## Topics

### Constants

case uint16

A 16-bit unsigned integer used as a primitive index.

case uint32

A 32-bit unsigned integer used as a primitive index.

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

enum MTLDepthClipMode

The mode that determines how to deal with fragments outside of the near or far planes.

enum MTLVisibilityResultMode

The mode that determines what, if anything, the GPU writes to the results buffer, after the GPU executes the render pass.

