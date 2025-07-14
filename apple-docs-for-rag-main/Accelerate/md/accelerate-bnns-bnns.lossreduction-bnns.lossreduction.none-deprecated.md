

- Accelerate
- BNNS
- BNNS.LossReduction
-  BNNS.LossReduction.none Deprecated

Case

# BNNS.LossReduction.none

Returns the loss without any reduction.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
case none
```

Deprecated

Use the BNNSGraph API instead.

## See Also

### Loss Reduction Functions

case reductionMean

Sums the loss of all samples in the batch and divides by the number of samples.

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

