

- Metal
- MTLCommonCounterSet
-  stageUtilization 

Type Property

# stageUtilization

The common name for the counter set that contains hardware utilization measurements from various render stages.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
static let stageUtilization: MTLCommonCounterSet
```

## Mentioned in 

Converting a GPU’s Counter Data into a Readable Format

## Discussion

The stage utilization counter set contains the following counters:

- totalCycles

- vertexCycles

- fragmentCycles

- tessellationCycles

- postTessellationVertexCycles

- renderTargetWriteCycles

Use this name to check whether a GPU device supports the corresponding counter set (see Confirming which Counters and Counter Sets a GPU Supports).

## See Also

### Common Counter Set Names

static let timestamp: MTLCommonCounterSet

The common name for the counter set that contains the timestamp counter.

static let statistic: MTLCommonCounterSet

The common name for the counter set that contains GPU workload statistics.

