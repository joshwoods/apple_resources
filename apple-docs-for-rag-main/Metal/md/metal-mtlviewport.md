

- Metal
-  MTLViewport 

Structure

# MTLViewport

A 3D rectangular region for the viewport clipping.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct MTLViewport
```

## Topics

### Creating a Viewport

init()

Returns a new viewport.

init(originX: Double, originY: Double, width: Double, height: Double, znear: Double, zfar: Double)

Returns a new viewport of a specified size at a specified origin.

### Specifying Viewport Boundaries

var originX: Double

The x coordinate of the upper-left corner of the viewport.

var originY: Double

The y coordinate of the upper-left corner of the viewport.

var width: Double

The width of the viewport, in pixels.

var height: Double

The height of the viewport, in pixels.

var znear: Double

The z coordinate of the near clipping plane of the viewport.

var zfar: Double

The z coordinate of the far clipping plane of the viewport.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Dynamic Render Pipeline States

struct MTLScissorRect

A rectangle for the scissor fragment test.

struct MTLVertexAmplificationViewMapping

An offset applied to a render target index and viewport index.

struct MTLQuadTessellationFactorsHalf

The per-patch tessellation factors for a quad patch.

struct MTLTriangleTessellationFactorsHalf

The per-patch tessellation factors for a triangle patch.

