

- Accelerate
- BNNS
- BNNS.NormalizationType
-  BNNS.NormalizationType.batch(movingMean:movingVariance:) Deprecated

Case

# BNNS.NormalizationType.batch(movingMean:movingVariance:)

Batch normalization with optional moving averages.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
case batch(
    movingMean: BNNSNDArrayDescriptor?,
    movingVariance: BNNSNDArrayDescriptor?
)
```

Deprecated

Use the BNNSGraph API instead.

## See Also

### Normalization Types

case group(groupCount: Int)

Group normalization.

Deprecated

case instance(movingMean: BNNSNDArrayDescriptor?, movingVariance: BNNSNDArrayDescriptor?)

Instance normalization with optional moving averages.

Deprecated

case layer(normalizationAxis: Int)

Layer normalization.

Deprecated

