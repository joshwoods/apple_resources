

- Metal
-  MTLQuadTessellationFactorsHalf 

Structure

# MTLQuadTessellationFactorsHalf

The per-patch tessellation factors for a quad patch.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct MTLQuadTessellationFactorsHalf
```

## Overview

Refer to the Tessellation chapter of the Metal Programming Guide for further information.

## Topics

### Fields

init()

Returns a new per-patch tessellation factors structure.

init(edgeTessellationFactor: (UInt16, UInt16, UInt16, UInt16), insideTessellationFactor: (UInt16, UInt16))

Returns a new per-patch tessellation factors structure with the specified parameters.

### Instance Properties

var edgeTessellationFactor: (UInt16, UInt16, UInt16, UInt16)

The edge tessellation factors, with each index value providing the tessellation factor for a particular edge.

var insideTessellationFactor: (UInt16, UInt16)

The inside tessellation factors, with the value in index 0 providing the horizontal tessellation factor and the value in index 1 providing the vertical tessellation factor.

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

struct MTLVertexAmplificationViewMapping

An offset applied to a render target index and viewport index.

struct MTLTriangleTessellationFactorsHalf

The per-patch tessellation factors for a triangle patch.

