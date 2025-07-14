

- Metal
-  MTLCounterResultStageUtilization 

Structure

# MTLCounterResultStageUtilization

The data structure for storing the data you resolve from a stage-utilization counter set.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
struct MTLCounterResultStageUtilization
```

## Mentioned in 

Converting a GPU’s Counter Data into a Readable Format

## Overview

For steps that explain how to resolve data from a counter set, such as stageUtilization, see Converting a GPU’s Counter Data into a Readable Format.

## Topics

### Stage Utilization Values

var totalCycles: UInt64

The total number of cycles the GPU uses to run a pass.

var vertexCycles: UInt64

The number of cycles the GPU uses to run vertex shaders during a pass.

var tessellationCycles: UInt64

The number of cycles the GPU uses to run the tessellation stage during a pass.

var postTessellationVertexCycles: UInt64

The number of cycles the GPU uses to run post-tessellation vertex shaders during a pass.

var fragmentCycles: UInt64

The number of cycles the GPU uses to run fragment shaders during a pass.

var renderTargetCycles: UInt64

The number of cycles the GPU uses to write data to render targets during a render pass.

### Swift Support

init()

Creates a default stage-utilization result.

init(totalCycles: UInt64, vertexCycles: UInt64, tessellationCycles: UInt64, postTessellationVertexCycles: UInt64, fragmentCycles: UInt64, renderTargetCycles: UInt64)

Creates a stage-utilization result from utilization values.

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

struct MTLCounterResultStatistic

The data structure for storing the data you resolve from a statistic counter set.

var MTLCounterErrorValue: UInt64

A sentinel value for an entry in a counter sample buffer that indicates the entry’s data is invalid.

