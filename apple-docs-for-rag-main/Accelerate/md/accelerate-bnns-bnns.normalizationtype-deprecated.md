

- Accelerate
- BNNS
-  BNNS.NormalizationType Deprecated

Enumeration

# BNNS.NormalizationType

Constants that describe normalization types.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+visionOSwatchOS 7.0+tvOS 14.0+

``` source
enum NormalizationType
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Normalization Types

case batch(movingMean: BNNSNDArrayDescriptor?, movingVariance: BNNSNDArrayDescriptor?)

Batch normalization with optional moving averages.

case group(groupCount: Int)

Group normalization.

case instance(movingMean: BNNSNDArrayDescriptor?, movingVariance: BNNSNDArrayDescriptor?)

Instance normalization with optional moving averages.

case layer(normalizationAxis: Int)

Layer normalization.

