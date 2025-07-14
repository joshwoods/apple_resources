

- Metal
-  MTLVertexAmplificationViewMapping 

Structure

# MTLVertexAmplificationViewMapping

An offset applied to a render target index and viewport index.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.4+macOS 10.15.4+tvOS 16.0+visionOS 1.0+

``` source
struct MTLVertexAmplificationViewMapping
```

## Mentioned in 

Improving Rendering Performance with Vertex Amplification

## Topics

### Creating a View Mapping

init()

Initializes a default view mapping.

init(viewportArrayIndexOffset: UInt32, renderTargetArrayIndexOffset: UInt32)

Initializes a new view mapping.

### Specifying Mapping Offsets

var renderTargetArrayIndexOffset: UInt32

An offset into the list of render targets.

var viewportArrayIndexOffset: UInt32

An offset into the list of viewports.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Dynamic Render Pipeline States

struct MTLViewport

A 3D rectangular region for the viewport clipping.

struct MTLScissorRect

A rectangle for the scissor fragment test.

struct MTLQuadTessellationFactorsHalf

The per-patch tessellation factors for a quad patch.

struct MTLTriangleTessellationFactorsHalf

The per-patch tessellation factors for a triangle patch.

