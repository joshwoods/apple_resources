

- Accelerate
- BNNS
- BNNS.LossReduction
-  BNNS.LossReduction.reductionMean Deprecated

Case

# BNNS.LossReduction.reductionMean

Sums the loss of all samples in the batch and divides by the number of samples.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+visionOSwatchOS 7.0+tvOS 14.0+

``` source
case reductionMean
```

Deprecated

Use the BNNSGraph API instead.

## See Also

### Loss Reduction Functions

case none

Returns the loss without any reduction.

Deprecated

case sum

Sums the loss of all samples in the batch.

Deprecated

case weightedMean

Sums the loss of all samples in the batch and divides by the sum of all weights.

Deprecated

case zeroWeightMean

Sums the loss of all samples in the batch and divides by the number of non-zero weights.

Deprecated

