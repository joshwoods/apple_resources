

- Accelerate
-  BNNSLossReductionNonZeroWeightMean 

Global Variable

# BNNSLossReductionNonZeroWeightMean

Sums the loss of all samples in the batch and divides by the number of non-zero weights.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var BNNSLossReductionNonZeroWeightMean: BNNSLossReductionFunction { get }
```

## Discussion

BNNSLossReductionNonZeroWeightMean sums the loss of all samples in the batch and divides by number of non-zero weights.

Non-zero weighted mean reduction returns 0 in case all weights are zero.

## See Also

### Reduction Functions

var rawValue: UInt32

init(UInt32)

init(rawValue: UInt32)

var BNNSLossReductionMean: BNNSLossReductionFunction

Sums the loss of all samples in the batch and divides by the number of samples.

var BNNSLossReductionSum: BNNSLossReductionFunction

Sums the loss of all samples in the batch.

var BNNSLossReductionWeightedMean: BNNSLossReductionFunction

Sums the loss of all samples in the batch and divides by the sum of all weights.

var BNNSLossReductionNone: BNNSLossReductionFunction

Returns the loss without any reduction.

