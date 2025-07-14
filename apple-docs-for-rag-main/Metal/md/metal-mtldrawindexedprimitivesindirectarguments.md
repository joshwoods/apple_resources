

- Metal
-  MTLDrawIndexedPrimitivesIndirectArguments 

Structure

# MTLDrawIndexedPrimitivesIndirectArguments

The data layout required for drawing indexed primitives via indirect buffer calls.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct MTLDrawIndexedPrimitivesIndirectArguments
```

## Mentioned in 

Specifying Drawing and Dispatch Arguments Indirectly

## Overview

See also the drawIndexedPrimitives(type:indexType:indexBuffer:indexBufferOffset:indirectBuffer:indirectBufferOffset:) method.

## Topics

### Fields

init()

Returns a new data layout for drawing indexed primitives via indirect buffer calls.

init(indexCount: UInt32, instanceCount: UInt32, indexStart: UInt32, baseVertex: Int32, baseInstance: UInt32)

Returns a new data layout for drawing indexed primitives via indirect buffer calls, with specified parameters.

### Instance Properties

var baseInstance: UInt32

The first instance to draw.

var baseVertex: Int32

The first vertex to draw.

var indexCount: UInt32

For each instance, the number of indices to read from the index buffer.

var indexStart: UInt32

The first index to draw.

var instanceCount: UInt32

The number of instances to draw.

var indexStart: UInt32

The first index to draw.

var baseVertex: Int32

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

struct MTLDrawPrimitivesIndirectArguments

The data layout required for drawing primitives via indirect buffer calls.

