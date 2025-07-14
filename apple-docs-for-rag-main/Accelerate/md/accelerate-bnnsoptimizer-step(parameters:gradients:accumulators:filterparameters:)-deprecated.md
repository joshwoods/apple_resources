

- Accelerate
- BNNSOptimizer
-  step(parameters:gradients:accumulators:filterParameters:) Deprecated

Instance Method

# step(parameters:gradients:accumulators:filterParameters:)

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+watchOS 7.0+visionOS

``` source
func step(
    parameters: [BNNSNDArrayDescriptor],
    gradients: [BNNSNDArrayDescriptor],
    accumulators: [BNNSNDArrayDescriptor],
    filterParameters: BNNSFilterParameters?
) throws
```

**Required** Default implementation provided.

Deprecated

Use the BNNSGraph API instead.

## Default Implementations

### BNNSOptimizer Implementations

func step(parameters: [BNNSNDArrayDescriptor], gradients: [BNNSNDArrayDescriptor], accumulators: [BNNSNDArrayDescriptor], filterParameters: BNNSFilterParameters?) throws

