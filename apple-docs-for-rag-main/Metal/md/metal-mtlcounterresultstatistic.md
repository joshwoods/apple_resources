

- Metal
-  MTLCounterResultStatistic 

Structure

# MTLCounterResultStatistic

The data structure for storing the data you resolve from a statistic counter set.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
struct MTLCounterResultStatistic
```

## Mentioned in 

Converting a GPU’s Counter Data into a Readable Format

## Overview

For steps that explain how to resolve data from a counter set, such as statistic, see Converting a GPU’s Counter Data into a Readable Format.

## Topics

### Statistics Values

var tessellationInputPatches: UInt64

The number of tessellation patches a render pass sends to the tessellation stage.

var vertexInvocations: UInt64

The number of times a render pass calls any vertex shader.

var postTessellationVertexInvocations: UInt64

The number of vertices a render pass sends to a post-tessellation vertex shader.

var clipperInvocations: UInt64

The number of primitives a render pass sends to the clip stage.

var clipperPrimitivesOut: UInt64

The number of primitives the clip stage produces during a render pass.

var fragmentInvocations: UInt64

The number of times a render pass calls fragment shaders.

var fragmentsPassed: UInt64

The number of fragments a render pass sends to the visibility and blend stages because they pass the scissor, depth, and stencil tests.

var computeKernelInvocations: UInt64

The number of times a pass calls any compute kernel.

### Swift Support

init()

Creates a default statistics result.

init(tessellationInputPatches: UInt64, vertexInvocations: UInt64, postTessellationVertexInvocations: UInt64, clipperInvocations: UInt64, clipperPrimitivesOut: UInt64, fragmentInvocations: UInt64, fragmentsPassed: UInt64, computeKernelInvocations: UInt64)

Creates a statistics result from statistic values.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Counter Sample Data Output

Converting a GPU’s Counter Data into a Readable Format

Inspect and use the data within a GPU’s counter sample buffer by resolving it into a standard format.

struct MTLCounterResultTimestamp

The data structure for storing the data you resolve from a timestamp counter set.

struct MTLCounterResultStageUtilization

The data structure for storing the data you resolve from a stage-utilization counter set.

var MTLCounterErrorValue: UInt64

A sentinel value for an entry in a counter sample buffer that indicates the entry’s data is invalid.

