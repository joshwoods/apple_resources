

- Accelerate
-  BNNSLossReductionMean 

Global Variable

# BNNSLossReductionMean

Sums the loss of all samples in the batch and divides by the number of samples.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var BNNSLossReductionMean: BNNSLossReductionFunction { get }
```

## Discussion

BNNSLossReductionMean sums the loss of all samples in the batch and divides by number of samples.

## See Also

### Reduction Functions

var rawValue: UInt32

init(UInt32)

init(rawValue: UInt32)

var BNNSLossReductionNonZeroWeightMean: BNNSLossReductionFunction

Sums the loss of all samples in the batch and divides by the number of non-zero weights.

var BNNSLossReductionSum: BNNSLossReductionFunction

Sums the loss of all samples in the batch.

var BNNSLossReductionWeightedMean: BNNSLossReductionFunction

Sums the loss of all samples in the batch and divides by the sum of all weights.

var BNNSLossReductionNone: BNNSLossReductionFunction

Returns the loss without any reduction.

