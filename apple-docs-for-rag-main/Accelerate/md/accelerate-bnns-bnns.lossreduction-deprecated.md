

- Accelerate
- BNNS
-  BNNS.LossReduction Deprecated

Enumeration

# BNNS.LossReduction

An enumeration that describes loss reduction functions.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
enum LossReduction
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Loss Reduction Functions

case none

Returns the loss without any reduction.

case reductionMean

Sums the loss of all samples in the batch and divides by the number of samples.

case sum

Sums the loss of all samples in the batch.

case weightedMean

Sums the loss of all samples in the batch and divides by the sum of all weights.

case zeroWeightMean

Sums the loss of all samples in the batch and divides by the number of non-zero weights.

### Instance Properties

var bnnsLossReductionFunction: BNNSLossReductionFunction

The underlying loss reduction function structure.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

