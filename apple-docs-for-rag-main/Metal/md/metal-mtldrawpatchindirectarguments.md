

- Metal
-  MTLDrawPatchIndirectArguments 

Structure

# MTLDrawPatchIndirectArguments

The data layout required for drawing patches via indirect buffer calls.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct MTLDrawPatchIndirectArguments
```

## Mentioned in 

Specifying Drawing and Dispatch Arguments Indirectly

## Overview

See also the following methods:

- drawPatches(numberOfPatchControlPoints:patchIndexBuffer:patchIndexBufferOffset:indirectBuffer:indirectBufferOffset:)

- drawIndexedPatches(numberOfPatchControlPoints:patchIndexBuffer:patchIndexBufferOffset:controlPointIndexBuffer:controlPointIndexBufferOffset:indirectBuffer:indirectBufferOffset:)

## Topics

### Fields

init()

Returns a new data layout for drawing patches via indirect buffer calls.

init(patchCount: UInt32, instanceCount: UInt32, patchStart: UInt32, baseInstance: UInt32)

Returns a new data layout for drawing patches via indirect buffer calls, with specified parameters.

### Instance Properties

var baseInstance: UInt32

The first instance to draw.

var instanceCount: UInt32

The number of instances to draw.

var patchCount: UInt32

The number of patches in each instance.

var instanceCount: UInt32

The number of instances to draw.

var patchStart: UInt32

The patch start index.

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

struct MTLDrawPrimitivesIndirectArguments

The data layout required for drawing primitives via indirect buffer calls.

struct MTLDrawIndexedPrimitivesIndirectArguments

The data layout required for drawing indexed primitives via indirect buffer calls.

