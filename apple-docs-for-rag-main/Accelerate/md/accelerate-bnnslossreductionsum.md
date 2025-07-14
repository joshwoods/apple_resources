

- Accelerate
-  BNNSLossReductionSum 

Global Variable

# BNNSLossReductionSum

Sums the loss of all samples in the batch.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var BNNSLossReductionSum: BNNSLossReductionFunction { get }
```

## Discussion

BNNSLossReductionSum sums the loss of all samples in the batch.

## See Also

### Reduction Functions

var rawValue: UInt32

init(UInt32)

init(rawValue: UInt32)

var BNNSLossReductionMean: BNNSLossReductionFunction

Sums the loss of all samples in the batch and divides by the number of samples.

var BNNSLossReductionNonZeroWeightMean: BNNSLossReductionFunction

Sums the loss of all samples in the batch and divides by the number of non-zero weights.

var BNNSLossReductionWeightedMean: BNNSLossReductionFunction

Sums the loss of all samples in the batch and divides by the sum of all weights.

var BNNSLossReductionNone: BNNSLossReductionFunction

Returns the loss without any reduction.

