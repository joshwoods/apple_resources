

- Accelerate
- BNNS
- BNNS.NormalizationType
-  BNNS.NormalizationType.group(groupCount:) Deprecated

Case

# BNNS.NormalizationType.group(groupCount:)

Group normalization.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
case group(groupCount: Int)
```

Deprecated

Use the BNNSGraph API instead.

## See Also

### Normalization Types

case batch(movingMean: BNNSNDArrayDescriptor?, movingVariance: BNNSNDArrayDescriptor?)

Batch normalization with optional moving averages.

Deprecated

case instance(movingMean: BNNSNDArrayDescriptor?, movingVariance: BNNSNDArrayDescriptor?)

Instance normalization with optional moving averages.

Deprecated

case layer(normalizationAxis: Int)

Layer normalization.

Deprecated

