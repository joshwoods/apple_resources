

- Metal
-  MTLScissorRect 

Structure

# MTLScissorRect

A rectangle for the scissor fragment test.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct MTLScissorRect
```

## Topics

### Creating a Scissor Rectangle

init()

init(x: Int, y: Int, width: Int, height: Int)

### Specifying Scissor Boundaries

var height: Int

The height of the scissor rectangle, in pixels.

var width: Int

The width of the scissor rectangle, in pixels.

var x: Int

The x window coordinate of the upper-left corner of the scissor rectangle.

var y: Int

The y window coordinate of the upper-left corner of the scissor rectangle.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Dynamic Render Pipeline States

struct MTLViewport

A 3D rectangular region for the viewport clipping.

struct MTLVertexAmplificationViewMapping

An offset applied to a render target index and viewport index.

struct MTLQuadTessellationFactorsHalf

The per-patch tessellation factors for a quad patch.

struct MTLTriangleTessellationFactorsHalf

The per-patch tessellation factors for a triangle patch.

