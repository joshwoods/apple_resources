

- Accelerate
- BNNSLossReductionFunction
-  init(rawValue:) 

Initializer

# init(rawValue:)

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(rawValue: UInt32)
```

## See Also

### Reduction Functions

var rawValue: UInt32

init(UInt32)

var BNNSLossReductionMean: BNNSLossReductionFunction

Sums the loss of all samples in the batch and divides by the number of samples.

var BNNSLossReductionNonZeroWeightMean: BNNSLossReductionFunction

Sums the loss of all samples in the batch and divides by the number of non-zero weights.

var BNNSLossReductionSum: BNNSLossReductionFunction

Sums the loss of all samples in the batch.

var BNNSLossReductionWeightedMean: BNNSLossReductionFunction

Sums the loss of all samples in the batch and divides by the sum of all weights.

var BNNSLossReductionNone: BNNSLossReductionFunction

Returns the loss without any reduction.

