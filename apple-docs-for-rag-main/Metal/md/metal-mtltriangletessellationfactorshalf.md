

- Metal
-  MTLTriangleTessellationFactorsHalf 

Structure

# MTLTriangleTessellationFactorsHalf

The per-patch tessellation factors for a triangle patch.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct MTLTriangleTessellationFactorsHalf
```

## Overview

Refer to the Tessellation chapter of the Metal Programming Guide for further information.

## Topics

### Fields

init()

init(edgeTessellationFactor: (UInt16, UInt16, UInt16), insideTessellationFactor: UInt16)

### Instance Properties

var edgeTessellationFactor: (UInt16, UInt16, UInt16)

The edge tessellation factors, with each index value providing the tessellation factor for a particular edge.

var insideTessellationFactor: UInt16

The inside tessellation factor.

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

struct MTLQuadTessellationFactorsHalf

The per-patch tessellation factors for a quad patch.

