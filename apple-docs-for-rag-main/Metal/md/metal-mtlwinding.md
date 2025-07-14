

- Metal
-  MTLWinding 

Enumeration

# MTLWinding

The vertex winding rule that determines a front-facing primitive.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
enum MTLWinding
```

## Topics

### Constants

case clockwise

Primitives whose vertices are specified in clockwise order are front-facing.

case counterClockwise

Primitives whose vertices are specified in counter-clockwise order are front-facing.

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

enum MTLCullMode

The mode that determines whether to perform culling and which type of primitive to cull.

enum MTLPrimitiveType

The geometric primitive type for drawing commands.

enum MTLIndexType

The index type for an index buffer that references vertices of geometric primitives.

enum MTLDepthClipMode

The mode that determines how to deal with fragments outside of the near or far planes.

enum MTLVisibilityResultMode

The mode that determines what, if anything, the GPU writes to the results buffer, after the GPU executes the render pass.

