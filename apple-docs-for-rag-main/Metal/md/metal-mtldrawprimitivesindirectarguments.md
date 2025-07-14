

- Metal
-  MTLDrawPrimitivesIndirectArguments 

Structure

# MTLDrawPrimitivesIndirectArguments

The data layout required for drawing primitives via indirect buffer calls.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct MTLDrawPrimitivesIndirectArguments
```

## Mentioned in 

Specifying Drawing and Dispatch Arguments Indirectly

## Overview

See also the drawPrimitives(type:indirectBuffer:indirectBufferOffset:) method.

## Topics

### Fields

init()

Returns a new data layout for drawing primitives via indirect buffer calls.

init(vertexCount: UInt32, instanceCount: UInt32, vertexStart: UInt32, baseInstance: UInt32)

Returns a new data layout for drawing primitives via indirect buffer calls, with specified parameters.

### Instance Properties

var baseInstance: UInt32

The first instance to draw.

var instanceCount: UInt32

The number of instances to draw.

var vertexCount: UInt32

The number of vertices to draw.

var instanceCount: UInt32

The number of instances to draw.

var vertexStart: UInt32

The first vertex to draw.

var baseInstance: UInt32

The first instance to draw.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Render Compute Commands

protocol MTLIndirectRenderCommand

A render command in an indirect command buffer.

struct MTLDrawPatchIndirectArguments

The data layout required for drawing patches via indirect buffer calls.

struct MTLDrawIndexedPrimitivesIndirectArguments

The data layout required for drawing indexed primitives via indirect buffer calls.

