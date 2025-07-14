

- Metal
- MTLCommonCounterSet
-  statistic 

Type Property

# statistic

The common name for the counter set that contains GPU workload statistics.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
static let statistic: MTLCommonCounterSet
```

## Mentioned in 

Converting a GPU’s Counter Data into a Readable Format

## Discussion

The statistics counter set contains the following counters:

- computeKernelInvocations

- vertexInvocations

- fragmentInvocations

- fragmentsPassed

- tessellationInputPatches

- postTessellationVertexInvocations

- clipperInvocations

- clipperPrimitivesOut

Use this name to check whether a GPU device supports the corresponding counter set (see Confirming which Counters and Counter Sets a GPU Supports).

## See Also

### Common Counter Set Names

static let timestamp: MTLCommonCounterSet

The common name for the counter set that contains the timestamp counter.

static let stageUtilization: MTLCommonCounterSet

The common name for the counter set that contains hardware utilization measurements from various render stages.

